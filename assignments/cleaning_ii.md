# Overview
This assignment will give you practice cleaning real data about passengers on the doomed ocean liner RMS *Titanic*.

**This is an individual assignment. You are meant to write the code on your own. You are welcome to discuss *ideas* with other students (including on the class email list), but don't look at their code or show them yours.**

# Importing the Data
If you haven't already done so, download the (very large!) file https://files.lerner.co.il/pandas-workout-data.zip and unzip it. Open the resulting folder and then open the `data` folder inside that.

Upload `titanic3.xls` into a fresh Google Colab notebook.

Once it's done, in your notebook, make any necessary imports and then load the data into a DataFrame called `df`.

What's that? I told you how to read .csv and .json files, but not .xls? (This is an old Excel format; newer ones will be .xlsx.) Make a few guesses as to what function you might use to read the data. If you can't figure it out, try a web search. If that doesn't work, contact me or the TA.

# Cleaning the Data

Add code to your notebook to do each of the following:
1. Find the mean age of passengers.
2. For those passengers with `NaN` for their age, replace it with the mean age. Hint: use the method `fillna`.
3. Remove any rows with `NaN` in the `'fare'` or `'embarked'` columns.
4. In the `home.dest` column, replace any `NaN`s with the most common (mode) value in that column.

# Verifying Your Results

Add the following to the end of your notebook to verify that everything worked right:

1. Calculate the mean age again. It should be about the same as it was before. (The slight difference, many decimal places out, has to do with the way computers do floating point calculations.)
2. `df.isnull().sum()` should show nonzero numbers only in the `cabin`, `boat`, and `body` rows.
3. `df['home.dest'].value_counts()[0]` should be 626.

# Optional Challenge Problem

Get the file `celebrity_deaths_2016.csv` from the same zipfile. Find the average age of celebrities who died in June through October of that year (ignoring any for which no valid age is provided). This will take some research!

# What to Hand In
Hand in your notebook.