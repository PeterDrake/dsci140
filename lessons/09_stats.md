# Statistics: why?
* Describing a dataset with a couple of numbers is useful for making comparisons
* Get [Data for Stats](https://docs.google.com/spreadsheets/d/1TCOPtZxMWusuRyOgkgxrj318FlCXnWro6aRsR4_EOHI/edit?usp=sharing)
* Question: Are the numbers in column A larger, smaller, or about the same as the numbers in column B?
  * Without using Google Sheets to do any calculations, look at the numbers and guess

# Measures of central tendency
* Mean
  * Usual meaning of "average"
  * Add up the values and divide by the count
  * Three ways in Google Sheets:
    * Manual formula
    * `AVERAGE`
    * Lower right summary
  * Often called $\mu$ (Greek letter mu)
  * Heavily affected by outliers
    * What if we add a new, much larger value to the bottom of a column?
* Median
  * Midpoint of data
    * If there is no midpoint, take the mean of the middle two points
  * Unaffected by outliers
  * Two ways in Google sheets:
    * Sort the data and look in the middle cell
    * `MEDIAN`
* Mode
  * Most common element
  * Rarely useful

# Measures of dispersion
* Range
  * Difference between largest and smallest values
  * In Google Sheets, `MAX` minus `MIN`
  * Entirely determined by outermost two points
* Interquartile range
  * Quartiles
    * 1/4 of the data are smaller than the first quartile
    * 2/4 = 1/2 are smaller than the second quartile
      * Warm call: What's another name for the second quartile?
    * 3/4 are smaller than the third quartile
    * 4/4 are smaller than the fourth quartile
      * WC: What's another name for the fourth quartile?
    * In Google Sheets, `QUARTILE`
      * Demonstrate with column A
    * There are also percentiles, deciles, and other quantiles
  * Interquartile range (IQR) is the difference between the third and first quartiles
    * Challenge: find the IQR of columns A and B
  * IQR ignores outliers altogether
* Standard deviation and variance
  * Variance: How much do data points differ from the mean?
    * Plan A: Add up the differences
      * The sum is always zero!
    * Plan B: Add up the absolute values of the differences
      * This would, work, but ...
    * Plan C: Add up the squares of the differences
      * This is preferable for technical reasons. One is that the square (unlike absolute value) doesn't have a sharp corner, so we can do calculus with it
      * Add up the squares of the differences from the mean and divide by the count
      * Often written as $\sigma^2$ (Greek letter sigma, squared)
      * If you like a formula: $\sigma^2 = \frac{\displaystyle\sum_{i=1}^{n}(x_i - \mu)^2} {n}$
      * In Google Sheets, `VARP`
    * Sample vs population variance
      * If you have data for the entire population, the mean is the true parameter: the mean for the population
      * The mean of a sample is an *unbiased estimate* of the population mean
      * The variance (as we've defined it) of a sample is *not* an unbiased estimate of the population variance, because the sample points are a little closer to the sample mean than to the population mean
      * To adjust for this, the sample variance is $\sigma^2 = \frac{\displaystyle\sum_{i=1}^{n}(x_i - \mu)^2} {n-1}$
      * This matters more when $n$ is small
      * In Google Sheets, use `VAR` instead of `VARP`
  * Standard deviation
    * The units of variance are squared, so it's hard to understand "a mean of 20 meters, with a variance of 2.3 square meters"
    * Standard deviation ($\sigma$) is just the square root of the variance
    * In Google Sheets, `STDEVP` (population) or `STDEV` (sample)
