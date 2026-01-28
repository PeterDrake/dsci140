# Visualization
* Makes it easier to get big picture of data, spotting trends and outliers
  * Easier for most people!
* Copy [sample data](https://docs.google.com/spreadsheets/d/16izvqPs7SgRed4MNXve4ryO0IXlVGG9OneXzSGits7I/edit?usp=sharing)
* Select some data and `Insert > Chart`
* First, look at a bar chart
  * What are the axes?
  * What are the marks (each corresponding to a data point?)
    * What do the aspects of each mark (position, size, color, etc.) tell you?
* Common chart types
  * One-dimensional (one series of data)
    * Bar (horizontal or vertical)
      * Use when the independent variable is discrete
        * Independent vs dependent variable
    * Line
      * Use when the independent variable is time or something else continuous
    * Pie
      * Rarely use; emphasizes fractions of whole
      * Never use 3D pie
  * Two-dimensional
    * Scatter
      * Shows relationship between two variables
    * Multiple overlapping versions of one-dimensional charts
      * Also works with more than two dimensions
* Customizing charts in Google Sheets
  * Style
    * Purely cosmetic, but that can affect readability
  * Titles
  * Series
    * Useful to distinguish them
    * Use color, but don't depend on it
      * Some people are colorblind
      * Sometimes people look at things printed in black and white
  * Legend
    * Include column headers in initial selection to make this work
  * Axes
    * Largely cosmetic, but note log scale
  * Gridlines and ticks
    * Cosmetic, but can affect readability
* Practice
  * Get the [data on bicycles crossing Seattle's Fremont bridge](https://github.com/jakevdp/bicycle-data)
  * Sort the sheet by date -- surprisingly, it isn't already sorted!
  * Plot the total number of bicycles for each of the first 1000 times.
    * What kind of plot should you make?
    * Do it.
    * What patterns do you notice?
    * How do you explain them?
  * Do the same for the first 50000 times.
  * Optional challenge: How does the temperature correlate with the number of bicycles?
    * Describe what plot you would make
    * Do it