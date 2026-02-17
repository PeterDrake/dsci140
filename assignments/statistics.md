# Overview
This assignment will have you computing various descriptive statistics, and plotting a few charts, based on data about [abalone](https://en.wikipedia.org/wiki/Abalone).

**This is an individual assignment. You are meant to write the code on your own. You are welcome to discuss *ideas* with other students (including on the class email list), but don't look at their code or show them yours.**

# Importing the Data

You can find the data here:

https://archive.ics.uci.edu/dataset/1/abalone

Downloading it will get you a .zip file, which you must unpack. It contains three files:
* `abalone.data` (the data themselves)
* `abalone.names` (an explanation of the dataset, including what the columns mean)
* `index` (a listing of the three files)

To import the data into a Google Sheets workbook, you'll first need to rename `abalone.data` to `abalone.csv`.

You'll also need to find the column names and paste them into a new row above the numbers.

# Tasks
1. Create a table showing, for each of the columns (except `Sex`, which is categorical):
   * Min
   * Max
   * Mean
   * Median
   * Standard deviation (sample, not population)
2. Plot a histogram of `Length`.
3. Create a scatter plot of `Height` (vertical axis) vs `Length`.
4. Compute (in another labeled cell) the correlation between `Length` and `Height`.
5. In yet another labeled cell, list your secret number (which was given as feedback in the Formulas assignment).

# Optional Challenge Problem

On a second sheet in the same workbook, plot a histogram with two series: one for male abalone, one for female. You should be able to tell at a glance whether male abalone tend to be much larger than, much smaller than, or about the same size as females.

# What to Hand in

Hand in a link to your workbook.