# Overview
This assignment will give you practice cleaning some fabricated data.

**This is an individual assignment. You are meant to write the code on your own. You are welcome to discuss *ideas* with other students (including on the class email list), but don't look at their code or show them yours.**

# Importing the Data
Get [the .csv file](https://education.launchcode.org/data-analysis-curriculum/cleaning-spreadsheets/exercises/index.files/cleaning-data-practice.csv) and import it into a new Google Sheets notebook.

# Cleaning the Data
1. Rename the original tab `original`. Duplicate it and name the new tab `cleaned`. No future work will use the `original` tab.
2. In the `cleaned` tab, remove the second `email` column, because it just repeats the data from the first one.
3. Remove all rows with blanks. Here's an approach that worked for me:
   1. Add a new, temporary column that counts the nonblank cells in each row.
   2. Create a filter to display all of the rows that _don't_ have the right number of nonblank cells.
   3. Delete those rows (not just their content!).
   4. Remove the filter to restore the previous rows.
   5. Delete the temporary column you created in step i.
4. Deal with outlier transactions.
   1. Find all the rows where the transaction value is greater than or equal to $1 million.
   2. Copy those rows (and their headers) into a new tab called `suspicious`.
   3. Remove those rows from `cleaned`.

# Optional Challenge Problem
Remove all rows with invalid email addresses. A valid address must contain an `@`, but not start with one. Consider using `SEARCH` and `IFERROR`.

# What to Hand In
Hand in a link to your notebook.

As a comment with your handin in Google Classroom, also tell me the secret number we left as a comment on the Formulas assignment. (This to verify that you are seeing the assignment feedback.)

# Credits / Notes
The data file came from https://education.launchcode.org/data-analysis-curriculum/cleaning-spreadsheets/exercises/index.html.

In real life, a password should never be stored in a spreadsheet.
