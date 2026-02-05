# Overview
This assignment will give you practice creating charts in a spreadsheet. It deals with data about board games.

**This is an individual assignment. You are meant to write the code on your own. You are welcome to discuss *ideas* with other students (including on the class email list), but don't look at their code or show them yours.**

# Importing the Data
Import [`bgg_dataset.csv` from Kaggle](https://www.kaggle.com/datasets/andrewmvd/board-games). You will need to make an account (or connect with your LC Google account) to download the data.

Two of the columns, `Rating Average` and `Complexity`, are real numbers formatted with a comma in place of the decimal point (which is standard in some countries). To turn them into numbers, select a column and then use find and replace.

# Charts
Create the following charts, each in a new sheet:
* A scatter plot of rating average vs complexity. (In other words, rating average is on the vertical axis and complexity on the horizontal axis.)
* A scatter plot of rating average vs play time. Limit the horizontal axis to 480 minutes to exclude a couple of incredibly long games.
* A column chart of average play time vs year published. I had to use a pivot table to pull this off.

For scatter plots, reduce the size of the points to make the data easier to see.

All charts should have titles and labels on both axes.

# Points to Ponder
There's nothing to write or hand in about these, but see if you can figure out:
* Do more complex games get higher or lower ratings?
* Do longer games get higher or lower ratings?
* What's up with the vertical stripes in the rating vs play time chart?
* Speaking of play time, what the heck happened in 1979 and 2022?

# Optional Challenge Problem
Produce a bar chart of the number of games using each the 20 most common mechanics.

This is *very difficult* because all of the mechanics (Dice Rolling, Set Collection, etc.) used by a given game shop up as a list in one cell. I was able to fund a solution using `SPLIT`, `UNIQUE`, `FLATTEN`, and `COUNTIF`. You will need to do some internet research!

# What to Hand in
Hand in a link to your workbook.
