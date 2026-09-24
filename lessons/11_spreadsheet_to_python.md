# Writing a "Program" in Google Sheets
* [Pig](https://en.wikipedia.org/wiki/Pig_(dice_game))
  * Hand out dice, have each pair (or trio) of students play
* Flowchart
  * New turn
    * -> Playing
  * Playing
    * Roll 1 -> Lose
    * Roll 2-6 -> Playing
    * Stop -> Score
  * Score
    * -> New turn
  * Lose
    * -> New turn
* Demonstrate [my version](https://docs.google.com/spreadsheets/d/1T1YAFp0Vt66mw9MLfEP8eAn9S14yPMvblvv-oKUmoTw/edit?usp=sharing)
  * Class plays against me
* Go through formulas
  * Key step: File > Settings > Calculation > Iterative on, max iterations 1
    * Otherwise we can't have circular references
  * Checkboxes (just Boolean values you can toggle with a click)
  * Specific cells
    * Winner
    * New turn
    * Score
    * Lose
    * Current player
    * Die
    * Total
    * Score
* Look at [Python version](https://colab.research.google.com/drive/1v3BuypOae5-_EEFof5840srQ74SpHO4N?usp=drive_link)
* Key point
  * Spreadsheets make it easy to see the data, but hard to see control flow
  * With programming languages, it's the other way around
