* Continue with previous lesson, with students driving

# Strings
* Generally, if you have a Series (e.g., a DataFrame column) of strings, you can call string methods on them: `s.str.isdigit()`.
* This returns a Series of the corresponding results.
* Work through exercise 36
* Regular expressions
  * A way of specifying patterns for strings
    * Fantastic for things like "Is this an email address?"
  * str methods
    * `fullmatch(pattern)` (entire string matches)
    * `contains(pattern)` (pattern appears somewhere in string)
  * Things to put in regular expression strings
    * Individual characters
    * `[xyz]`: Any of these characters
    * `[A-Za-z]`: Any character in these ranges
    * `.`: Any one character
    * `^`: Beginning of string
    * `$`: End of string
    * `*`: Zero or more of the previous thing
    * `+`: One or more of the previous thing
    * `?`: Zero or one of the previous thing
    * `\d`: Any digit
    * `\s`: Any whitespace character
    * `\w`: Any letter, digit, or underscore
