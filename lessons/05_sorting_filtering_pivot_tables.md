# Sorting
* Copy [Sample Data](https://docs.google.com/spreadsheets/d/1NXHCX8-yD4GZiDAEidxQG2X1jzuqoHZPWD27fi8Oq6I/edit?usp=sharing)
* Be sure to freeze any header row first
* Select a *column*
* From the down arrow at the top of the column, `Sort sheet A to Z`
  * It will also sort the other rows!
  * Numbers and dates are sorted in the way you would expect
  * Text is sorted alphabetically -- ignores case
    * Other software, like Python, will do this differently
* Multiple sorts
  * Sort on the least important column first
  * Presidents example
    * Freeze column headers
    * Extract first names with `=INDEX(SPLIT(A2, " "), 2)`
    * Extract last names with `=INDEX(SPLIT(A2, " "), COUNTA(SPLIT(A2, " ")))`
    * Sort on first names
    * Sort on last names
    * Note that Benjamin Harrison is before William Harrison

# Filtering
0:30
* Click somewhere in a table and `ctrl-A` (`cmd-a` on a Mac) to select all of it
* Click on the funnel icon in the toolbar or `Data > Create a filter`
* Click the filter (striped triangle) at the top of a column
  * Sort
  * Filter by values
    * Unselecting one doesn't delete the data; it just hides it
  * Filter by condition

# Pivot tables
0:40
* Click in a cell and `Insert > Pivot Table`
* Pick one or more rows and one or more values
  * In iris example, try target and average of sepal length
* If you pick a row and a column, you get a 2D pivot table

# Interactive activity
0:50
* Create a 2D pivot table showing the average HP of the different types of Pokemon, legendary vs non-legendary
* Optional bonus challenge: visualize the results in a chart
