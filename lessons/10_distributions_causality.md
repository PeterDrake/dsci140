# Histograms
* Plot column A using same data from last time
* Looks like a bar chart
* Data are grouped into bins (buckets)
  * Experiment with bucket size
  * What happens if the bucket size is too large?
  * What if it's too small?

# Distributions
* Uniform
  * Histogram looks flat
  * Arieses when all outcomes are equally likely
    * Rolling one (fair) die
* Normal
  * Bell curve
    * Most values near mean, fewer the farther away you get
  * Arises when many independent factors contribute
    * Height
    * Sum of several dice
  * 68-96-99.7 rule
    * Verify this
* Exponential
  * Tall with a long tail
  * Arises in "rich get richer" situations
    * Wealth
    * Popularity (songs, movies, books, social media posts)

# Correlation
* Make scatter plot of x and y columns in "Correlation" tab
* We say these are *positively correlated* because, when one goes up, the other also goes up
* Pearson's correlation coefficient ranges from -1 to 1
  * https://en.wikipedia.org/wiki/Correlation#/media/File:Correlation_examples2.svg
  * Note that slope isn't a big factor here (except sign)
  * Closer to +/- 1 means tighter, closer to a line
* In Google Sheets, use `CORREL`

# Causality
* If two variables are highly correlated, does that mean changing one would affect the other (e.g., participating in Chess club and SAT scores)?
* https://www.tylervigen.com/spurious-correlations
* https://xkcd.com/552/
* Possible reasons for correlation between A and B
  * Coincidence (statistics can help rule this out) 
  * A causes B
  * B causes A
  * They're both caused by a third common factor
  * Team discussions: Give an explanation for each of the last three for the relationship between smoking and lung cancer
* How to tell if it's causality
  * The future cannot cause the past
  * Is there a mechanism?
  * Controlled, replicated experiments
