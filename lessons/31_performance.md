# Performance
* Performance means using no more time or memory than necessary
  * Time matters if it's not fast enough
    * For some problems, speed can make the difference between "instant" and "hours", or between "hours" and "longer than the expected lifespan of the universe"
  * Memory ("space") matters if you don't have enough
    * Using less memory can improve speed because of caches
  * Consider tradeoffs between *development* time and *running* time
  * Performance matters when the problem is large
    * Lots of data
      * Loading time can be significant
      * Discussion: What if the data don't fit in memory?
    * Combinatorial explosions
      * Activity:
        * How many arrangements of a deck of playing cards have appeared in history?
          * Make reasonable assumptions for back-of-envelope calculation
            * Years since invention of playing cards
            * Population of Earth
            * Everyone shuffles once per minute
        * How many arrangements are possible?
        * What are the odds that a given arrangement has appeared before?
* Timing code
  * In Jupyter, begin cell with `%%timeit`
  * Generate a Series of 1,000,000 random numbers and add them up
    * Using a for loop and raw Python
    * Using the `sum` method on the Series
  * When analyzing algorithms, timing of one particular data set may not be representative
    * For example, sorting a series that is already sorted (or close to it) may be faster than sorting a random or reverse-sorted list
    * Analysis of algorithms provides some mathematical tools for dealing with this
* General hints
  * Omit needless computation
    * Don't compute values you don't need
    * Don't repeat computations
      * If you're going to use something again, save it!
  * Load only the data you need
  * Avoid raw Python iterations (`for` loops, list comprehensions) on Series and DataFrames
  * Use broadcasting
  * Use the smallest dtype you can
  * Use categories for columns with repeated values
  * Consider loading and saving in a binary format like feather
    * Drawback: less interoperability
* Work through exercise 48, continuing to "beyond" challenges if time permits
