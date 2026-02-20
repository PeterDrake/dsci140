# Jupyter (Google Colaboratory) Notebooks
* Interactive notebook
* Code cells
  * Running them
* Text cells
  * Some formatting is available
* Experiment: What if you put several expressions in a cell and run it?

# Data Types
* Every value (object) has a type
* The `type` function returns the type of a value.
* Experiment: What are the types of the following values?
  * 5
  * 'hello'
  * 2.718
  * True
* Lists
  * Enclosed in square brackets, with the elements separated by commas
  * Elements can be any type
    * Experiment: Do all elements of a list have to be the same type?
    * Experiment: Can you make a list of lists?
  * Most things you did with strings (len, slicing, addition) also work with lists
* Type conversion
  * The name of a type is also the name of a function that converts something to that type
  * Team experiment: For each of the five types, try converting it to each of the other types. Draw on your whiteboard a table indicating if it's possible:
    * Yes
    * No
    * It's complicated (only sometimes or something special happens)
* There are many more types, and it's even possible to define your own

# Variables
* Define variables with `=`
* Python variable names are conventionally `snake_case`, but this is not enforced
  * Experiment: Are `x` and `X` the same variable?
* Experiment: If you define a variable in one cell, is it visible in the next? Is it visible in a previous cell?
  * Order of running matters!
  * `Runtime > Run all` and `Runtime > Run before`
* Experiment: If you define a variable with a value of one type, can you redefine it with a value of another type?
* Experiment: What happens if you redefine one of the built-in functions and then try to use it?
  * Recovering with `Runtime > Restart session`
* Challenge: Define a list `my_list`. In each of several later cells, define `i` and get element `i` of the list. You should be able to redefine the list and re-run everything to do the same processing on a different list.
* Challenge: Write a cell that determines if a word is a palindrome. You should be able to check a different word just by changing a variable.


