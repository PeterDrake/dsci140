# Review

## General Concepts
* What is data science?
* Structures vs unstructured data
* Data types
  * NOIR
  * Text
  * Images
  * Maps, trees, and graphs
* File formats
  * CSV
  * JSON
* Measurement issues
  * Definitions
  * Units
  * Accuracy
  * Bias
* Cleaning data
  * Missing data
  * Duplicates
  * Inconsistent formatting
  * "Erroneous" data
* Visualization
  * Data points are represented by marks (lines, dots, etc.) on a chart
  * Attributes are represented by position, color, size, shape, etc.
  * Types of plots
    * Scatter
    * Line
    * Bar
    * Histogram
    * Box

## Spreadsheets
* Name three pieces of spreadsheet software
* Workbooks, sheets, and cells
* Rows and columns
* Formulas
  * Automatically updated whenever anything changes
* Absolute vs relative references
* Sorting and filtering
* Pivot tables
* Primitive visualization

## Statistics
* Population vs sample
  * Parameter vs statistic
  * Simple random vs stratified
* Measures of central tendency
  * Mean
  * Median
  * Mode
* Measures of dispersion
  * Range
  * Interquartile range
  * Standard deviation and variance
    * Population vs sample
* Distributions
  * Uniform
  * Normal
  * Exponential
* Correlation and causality

## Python
[Ten Eternal Truths About Python](https://docs.google.com/presentation/d/1OQ7YHJqNgGblz9GVC6l80wyomk1NoFTfGqOBAzr-Mpc/edit?usp=sharing)

## Pandas
* Series, DataFrames, and Indexes
* Importing and exporting data
* Typical pandas program:
  ```python
  import pandas as pd
  df = pd.read_csv('data.csv')
  df = df.method().method().method()
  df.method().method().method()
  ```
* Most methods return a new DataFrame (or Series) rather than modify an existing one
* Access parts of a DataFrame with `df.loc[rows, columns]`
* Many operations work on entire Series or DataFrames
* Boolean Series can be used as mask indices
* Grouping, joining, sorting, and pivot tables
  * Left, inner, and outer joins
* `.str` accessor to perform string operations
* `Timestamp` and `Timedelta`
* Visualization
  * Matplotlib
  * Pandas
  * Seaborn
* Performance hints
  * Omit needless computation (and data)
  * Avoid raw Python iteration
  * Use smaller data types
