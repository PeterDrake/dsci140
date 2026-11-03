# Data Frames
* Before we start, start downloading the [data](https://files.lerner.co.il/pandas-workout-data.zip), as it will take a while
* A pandas DataFrame is like a spreadsheet
  * Each column is a series
  * One way to create one is to provide `DataFrame` with:
    * The data as a list of lists (one per row)
    * `index=`, an optional list of index (row) names
    * `columns=`, an optional list of column names
  * Alternatively, you can pass a list of dicts (one per row)
* You can refer to columns as if you were looking things up in a dictionary, e.g., `df['temperature']`
* Lerner exercise 8 solution
  * Alternatively, you can add a new column `'net_profit'`
* To refer to rows, use either `iloc` or `loc`, just like with a series
  * If you provide two "arguments" (row and column) inside square brackets to one of these, you get an individual cell
  * Either of these can be a list
  * It can also be a sequence of bools, as you might get as the result of a comparison
* Lerner exercise 12 solution
