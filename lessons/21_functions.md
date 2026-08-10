# Defining Functions
* In addition to naming data, you can name computations!
* General form
  ```python
  def name(argument, ...):
    statement
    ...
  ```
* `return` statement
  * Once you return, you exit the function
  * A function might be written to return a value, have a side effect, or (rarely) both
  * Experiment: What is returned by a function with no `return` statement?
* Challenge: Define `my_max`
  * Don't use the built-in `max`; use iteration
* Remember that, as with any other definition, you have to re-run the cell if you change the code!
* Testing functions
  * What to test?
    * One input
    * All possible inputs
    * A random sample
    * A sample that hits important cases
  * Automating tests with `assert` statements
* More challenges
  * `my_sum`
  * `my_mean`
  * `my_median`
    * You can use `sorted`
    * Be sure to account for even or odd length lists
  * `my_variance`
    * Use the formula for sample variance, not population variance
  * `my_standard_deviation`
    * One way to take a square root is to raise a number to the power 0.5
* Advanced challenge
  * Write a function to recognize each type of Poker hand
  * Then write a function that, given a hand, determines the strongest category it's in
  * Finally, write a function that, given *two* poker hands, determines which is stronger, including breaking ties with higher cards
