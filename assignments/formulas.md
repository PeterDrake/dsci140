# Overview
This assignment will give you practice using formulas in a spreadsheet. It deals with [data about penguins found in the Palmer Archipelago off the coast of Antarctica](https://github.com/allisonhorst/palmerpenguins).

**This is an individual assignment. You are meant to write the code on your own. You are welcome to discuss *ideas* with other students (including on the class email list), but don't look at their code or show them yours.**

# Importing the Data
1. Start at https://gist.github.com/slopp/ce3b90b9168f2f921784de84fa445651#file-penguins-csv.
2. Click on the `Raw` button at the upper right of the table to see the raw file without the web page formatting.
3. Use `Save Page As` in your web browser to save this file as `penguins.csv`.
4. Create a Google Sheet called `Penguins`.
5. Import the data into the sheet (`File > Import`, then find the `Upload` tab). For the import location, choose `Replace current sheet`.

# New Columns
Note: Some cells in the data say `NA` (not available). For this assignment, we'll just ignore these values. Functions like `SUM` and `AVERAGE` also ignore them. If you write a formula that depends on a specific `NA` value, you'll get `#VALUE!`, which is fine for now. We'll talk about missing data later in the course.

Add the following new columns:
1. `bill_length_inches`, computed from `bill_length_mm` by dividing that column by 25.4.
1. `bill_volume_mm^3`, which will represent the approximate volume of the penguin's bill in cubic millimeters. To compute this, we will assume that the bill is a cone. The volume of a cone is $\frac{\pi r^2 h}{3}$. Use `bill_length_mm` for $h$ and half of `bill_depth_mm` for $r$. Use `PI()` for $\pi$.

Don't share your *formulas* with classmates, but feel free to compare your first couple of *results*.

# Extracting Information
1. Add the label `Longest bill` in cell M3.
1. In cell N3, use a formula to find the length (in mm) of the longest bill of any of these penguins.
1. In cell M4, add the label `Year found`.
1. In cell N4, use `VLOOKUP` to find the year that the penguin with the longest bill was found.
1. In cell M5, add the label `Females`.
1. In cell N5, compute the percentage of the penguins that are marked as female. `COUNTIF` and `COUNTA` are helpful here.

# Formatting
1. Make the top row (the column headers) bold and centered.
1. Freeze the top row.
1. In your two new columns, reduce the number of digits so that only one after the decimal point is displayed.
1. Display the percentage of females in cell N5 as a whole number percentage.
1. Resize the columns to fit the data.

# Optional Challenge Problem
Create a second sheet (in the same workbook) and show the minimum, average, and maximum body mass of the penguins of each species. You may need to research functions we haven't discussed!

# What to Hand in
Hand in a link to your workbook.