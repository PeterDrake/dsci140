* Again, challenges for students to work out

# Grouping
* Using `groupby`, determine how many skyscrapers are in each city
  * Give the results in descending order by city

# Joins
* Concept of joins
* Examples of each of the four types from my solution to `skyscrapers.ipynb`
* Load `cities.json` into a dataframe `cities`
* Fixing the missing latitude and longitudes in original skyscrapers dataframe `df`
  * Plan:
    * Make a dataframe `missing` of just those buildings with missing latitude
    * Join this with `cities` into a new dataframe `combined`
    * Replace the bad column `location.latitude` with `latitude`; similarly with longitude
    * Concatenate the rows from `df` that *do* have valid lat/long with `combined` to get a new, clean dataset
  * Complications:
    * Joining works on indices
      * Solution: set the indices of both `missing` and `cities`
        * Remember to reset after the join
    * The join has more rows than `missing`!
      * How could this happen?
      * Solution: sort `cities` in descending population order and remove duplicates
    * `cities` says `New York` instead of `New York City`
      * Rename those index elements with `rename`
    * Some cities still aren't handled
      * Drop, ignore, or fix manually
* Make the scatter plot map again
  * Why aren't the cities we didn't fix plotted?