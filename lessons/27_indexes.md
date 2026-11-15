# Indexes
* A Series has one Index
* A DataFrame has one Index for rows ("the" index) and one for columns
* An index object can be converted into a list
* `set_index` and `reset_index`
* Work through [Lerner's exercise 21](https://github.com/reuven/pandas-workout/blob/main/chapter-04/Exercise%2021%20%E2%80%94%20Parking%20tickets.ipynb)
* Multi-indexes are hierarchical, e.g., year and then month
  * `loc` can take a tuple to specify a place in such an index
  * [Exercise 22](https://github.com/reuven/pandas-workout/blob/main/chapter-04/Exercise%2022%20%E2%80%94%20SAT%20scores.ipynb)

# Pivot Tables
* Idea is the same as in spreadsheets
  * Pick three columns:
    * Rows will be different values from the `index` column
    * Columns will be different values from the `columns` column
    * Values will be means of all corresponding values of `values` column
      * You can supply an optional `aggfunc` to get something like `'max'` or `'size`' instead of mean
* [Exercise 24](https://github.com/reuven/pandas-workout/blob/main/chapter-04/Exercise%2024%20%E2%80%94%20More%20Olympic%20stats.ipynb)
