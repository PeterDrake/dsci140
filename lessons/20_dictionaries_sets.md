# Discuss Defense Against Dishonest Charts

# Dictionaries
* A dictionary associates *keys* with *values*
* Example: names and ages
* A dictionary can be used to represent a two-column table
* Create an empty dict with `{}`
* Accessing and setting entries
  * It's sort of like a list, but with keys instead of indices
* Two keys can have the same value, but each key only has one value
  * If you write to an existing key, the old one is replaced
* Operations
  * `len`
  * Iterate through keys with for loop or list comprehension
  * Methods: `.keys`, `.values`, `.items`
    * `.items` give you a list of *tuples*
* Predict and then try: What happens if you convert a dictionary into a list?
* Challenge: Write code to find the sum of the *values* in a dictionary
* Challenge: Given a list of words, create a dictionary associating words with their lengths

# Sets
* A collection of items
  * Like a list, but
    * Order doesn't matter
      * Small numbers may be displayed in order, but you can't count on this
    * No duplicates
* Example: numbers
* Create an empty one with `set()`
  * `{}` creates a dict
* Add items with `.add`
* Remove items with `.remove`
* Use `in` to check membership
* Operations
  * `&` for intersection
  * `|` for union
* `len` works and sets are iterable
* Challenge: Create a set of multiples of 2 and a set of multiples of 3, then combine them to create a set of multiples of 6
* Challenge: Given a list with duplicates, use type conversion to create a list with the duplicates removed
* Experiment: What types of objects can be members of sets? What types can be keys in dictionaries? What types can be values in dictionaries?
