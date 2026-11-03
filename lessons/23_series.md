# Series
* Adapted from Lerner, *Pandas Workout*, Exercise 1
* A pandas *series* is like one column in a spreadsheet
* The challenge
  * Create a series of 10 random integers from 70 to 100 (monthly exam scores), indexed by month from September through June.
  * What is the student's average test score?
  * What is the average for the first five months?
  * The second five months?
  * Did they improve or get worse in the second half? How much?
* Random scores
  * `import numpy as np` 
  * `import pandas as pd`
  * `g = np.random.default_rng(0)`
    * The 0 is a (pseudo)random number generator seed, so we all get the same numbers
    * [Epic tale of suspicious data](https://pubpeer.com/publications/EFB5C468100FD85BE8CC935CC960F7)
  * `s = pd.Series(g.integers(70, 101, 10))`
* Indexing on months
  * `months = 'Sep Oct Nov Dec Jan Feb Mar Apr May Jun'.split()`
    * Notice how we used `split` to avoid typing a bunch of commas!
  * `s = pd.Series(g.integers(70, 101, 10), index=months)`
* Yearly average
  * `s.mean()`
    * Other methods include `max`, `min`, `median`, `std`
* Taking parts of the series
  * `s.iloc[:5]`
    * `s.iloc[:5].mean()`
      * Notice how we've chained steps with `.` -- this is very common in pandas!
    * `iloc` means "integer location", using the integer position
  * `s.loc['Sep':'Jan']`
    * `loc` uses the series's actual, explicit index
    * Unlike `iloc` and normal Python slices, this *does* include the index after the column
      * That's because "up to but not including" might not make sense for some indices
  * Challenge: Compute the average for the second half of the year
  * Challenge: Compute the improvement from first to second half
* Bonus challenges
  * In what month did the student get their highest test score?
    * Plan A: Use the `sort_values` method
    * Plan B: Create a boolean mask that finds out the maximum score, then use that to find an element
      * Because there might be several, take the first one
  * What were the student's five highest scores?
    * Sort and slice!
  * Round each score to the nearest 10 points
    * Use the `round` method. Experiment with what its optional integer argument does. What if it was negative?