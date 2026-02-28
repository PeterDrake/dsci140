# Iteration
* To iterate is to repeat. Python has various structures for telling the computer to repeat instructions multiple times.

## While Loops
* This is the simplest and most general-purpose loop.
  ```python
  while condition:
    statement
    ...
  ```
* Example: counting from 1 to 10
* Challenge: count *down* from 10 to 1
* Example: printing the elements of a list
* Creating an infinite loop
* `break`
  * Exits the loop
  * Example: get a series of numbers from user, then print their sum
    * Requires introducing `if`
  * Challenge: get a series of numbers from the user and stop after the first duplicate
    * You will need `in`, which works differently for strings and lists
* `continue`
  * Skips the rest of the current pass through the loop and continues from the top
  * Example: add up a list of numbers, skipping any negative ones

## For Loops
* More convenient for the common situation where you're iterating through a list, string, or other structure
  ```python
  for variable in iterable:
    statement
    ...
  ```
* On each pass through the loop, `variable` is a name for one element of iterable
* `range` for iterating through numbers
  * Examples: counting up and down
* Many of the previous examples are more concise with a for loop
* Nesting loops
  * Example: all pairs of an element from one list and an element from another
  * Challenge: print a multiplication table

