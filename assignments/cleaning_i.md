Create "original", "cleaned" tabs
Redundant email column
Remove rows with blanks
    Add a new column that counts the nonblank cells in each row
    Create a filter to display all of the rows that don't have the right number of cells
    Delete those rows
    Remove the filter to restore the previous rows
    Remove the temporary column you created in step b
Outlier transactions
    Find all of the rows where the transaction value is >= $1M
    Copy those rows (with their headers) into a new tab "suspicious"
    Remove those rows from "cleaned"
Bad email addresses (optional)
    Must contain an @, but not start with an @
        Consider using SEARCH and IFERROR

    