# Formulas
* Create a new sheet (or use the one from last time) for simple experiments
* `=2+2`
  * Note difference between the formula and the value it computes
  * Arithmetic operators: `+`, `-`, `*`, `/`
  * Comparison operators: `<`, `<=`, `=`, `>=`, `>`
    * `<>` means "not equal to"
  * Concatenate strings with `&`
* Referring to an existing cell
  * It's automatically updated when the data changes
  * References are changed when you copy to another cell
  * Absolute vs relative references
    * F4 to toggle variations
* Getting the sum of a range with `SUM`
* `COUNT`
  * Challenge: compute average using these two
* `AVERAGE` and `MAX`
* `RANDOM`
  * It's updated any time you edit anything
  * Copy and paste values
* `IF`
* Nesting formulas
* `VLOOKUP(A2, $B$10:$C$15, 2, FALSE)`
  * Looks *for* whatever is in A2
  * Looks *in* the first column of the specified range
  * Returns the corresponding value in column 2 (relative, 1-based) within the range
  * You always want FALSE
    * TRUE is an "approximate match" and assumes the data are sorted
* [Google Sheets function cheat sheet](https://docs.google.com/spreadsheets/d/1AqN6OMBf5Gzo7D4LTv9uQtqLHQC1d3BPSnquSLhjWfw/edit?usp=sharing)
## Interactive Activities
* You can find a Google Sheet or import a xlsx, ods, or csv file
* Open [Billboard Hot 100 Number Ones Database](https://docs.google.com/spreadsheets/d/1j1AUgtMnjpFTz54UdXgCKZ1i4bNxFjf01ImJ-BqBEt0/edit)
* Make a copy so you can edit
  * Create a new sheet
  * Refer to cells in another sheet as, for example, Data!A1
* `VLOOKUP` example: When did BTS's "Butter" hit #1?
* Average BPM
* Average BPM within each decade
  * What are your instincts?
  * Add a Year column to data sheet
    * To copy a formula down the whole column:
      * Select it
      * Ctrl-shift-down
      * Ctrl-enter
  * Add a Decade column
  * Add a new column for the BPM of each decade
  * Average these in the other sheet
* What other questions would people like to explore?

