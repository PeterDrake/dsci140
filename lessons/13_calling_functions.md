# Calling Functions
* `function(argument, ...)` passes the arguments to the function and returns a value
* Some built-in functions
  * `abs`
  * `all`
  * `any`
  * `help`
    * Prints something as a side effect
    * Return value is `None`, which isn't printed
      * Experiment: What is the type of `None`?
  * `input`
    * Asks for user input
    * Optional prompt argument
    * Returned value is a str
  * `len`
  * `max`
  * `min`
  * `print`
    * Like `help`, prints as a side effect and returns `None`
  * `round`
  * `sorted`
  * `sum`
  * `type`
  * Type conversion functions like `int`, `float`, `str`, `bool`, `list`
  * There is a [complete list](https://docs.python.org/3/library/functions.html), but a few of them are obscure

# Calling Methods
* Example: `'hello'.upper()`
* `object.method(argument, ...)` passes the arguments to the method (called on the object) and returns a value
  * Why? Some methods behave differently (obviously or behind the scenes) when called on different types of objects

## String methods
* [Complete list](https://docs.python.org/3/library/stdtypes.html#string-methods)
* Alternatively (but more concisely), `help(str.upper)`
* `count`
* `endswith`
* `index`
* `isalpha` and related methods
* `join`
* `lower`
* `replace`
* `split`
* `startswith`
* `strip`
* `upper`

## List methods
* Lists, unlike strings, are *mutable*, so some methods modify the list
* [Complete list](https://docs.python.org/3/tutorial/datastructures.html#more-on-lists)
* `append`
* `count`
* `extend`
* `index`
