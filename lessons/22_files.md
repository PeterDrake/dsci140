# Text Files
* Getting files into a Google Colab notebook
  * Let's start at [Project Gutenberg](https://www.gutenberg.org/)
    * How about *Frankenstein*?
      * Be sure to get the plain text file
  * Upload the file to your notebook
    * Pay attention to that warning -- files go away when your runtime cuts out!
  * You can view (or even edit) a plain text file within the notebook, but you'll have to download it if you want to keep it around
* Printing some lines from a file
  ```python
  with open('frankenstein.txt') as file:
    for i in range(10):
      line = file.readline()
      print(line)
  ```
  * Better yet, `print(line.strip())` to remove whitespace, including end-of-line artifacts
* Alternatively, just call `file.readlines()` to get a list of all the lines
  * This may not work with extremely large files, as it has to store the whole file in memory
* Challenge: Print the first paragraph of the novel
  * You get to know that the first line starts with `'You will rejoice'`.
  * You know you're at the end of the paragraph when you find a blank line.
* Writing to files
  ```python
  with open('poem.txt', 'w') as file:
    file.write('The fish has too many bones,\n')
    file.write('and the watermelon too many seeds.\n')
    file.write('- Charles Reznikoff\n')
  ```
* Challenge: Write an all-caps version of Frankenstein to a new file.

# CSV Files
* Handily, Google Colab provides a couple of examples in the `sample_data` directory
  ```python
  import csv

  with open('sample_data/california_housing_test.csv') as file:
    data = list(csv.DictReader(file))

  data[:5]
  ```
  * You can look at (and edit) the CSV file within the notebook
* It's a list of dicts!
* Challenge: How many data points are in this file?
* Challenge: Find the average longitude and latitude of the houses in this dataset
  * Then we'll use openstreetmap.org to verify that this location is in California
* Challenge: Manually build a small dict and write it to a file