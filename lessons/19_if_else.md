## List Comprehensions
* Most convenient when you want to perform some operation on each element of a list
* `[variable for variable in iterable]`
* Example: doubling the numbers in a list
* Fancy variant: `[variable for variable in iterable if condition]`
* Challenge: list of all prefixes of a string

## If
* Decide what to do based on a boolean condition
* Simple form: one-armed if
  ```python
  if condition:
    statement
    ...
  ```
  * Example: print all addresses starting with 'S ' in a list of strings
* Two-armed if
  ```python
  if condition:
    statement
    ...
  else:
    statement
    ...
  ```
  * Example: censor certain words in a sentence
* Multiple branches
  ```python
  if condition:
    statement
    ...
  elif condition:
    statement
    ...
  ...
  else:
    statement
    ...  
  ```
  * Example: is a temperature cold, medium, or hot?
* Nesting
  * Example: choose clothing for top/bottom and warm/cold
* Mob program: rock/paper/scissors
  * Uses `random.choice`
* Challenge: number guessing game
  * Uses `random.randint`
  * Elite version: the computer does the guessing
