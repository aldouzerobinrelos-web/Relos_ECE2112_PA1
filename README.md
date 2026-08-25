# Relos_ECE2112_PA1
The content of this repository contains Programming Assignment 1 for the course Advance Computer Programming

# 1. WORD ROTATION PROBLEM
Create a function named rotate word() that accepts a non-empty string. Move the first character of the string to the end while keeping all remaining characters in their original order. Preserve the capitalization of every character.

The following function and string operations were used in this problem:

`def rotate_word(text)` - defines a function named `rotate_word` with `text` as its parameter. The parameter receives the string provided when the function is called.

`text[0]` - uses indexing to access the first character of the string.

Example:

`"python"[0]` --> `"p"`

`text[1:]` - uses slicing to obtain the characters beginning from the second character up to the end.

Example:

`"python"[1:]` --> `"ython"`

These two parts are then joined together using the `+` operator. The sliced portion is placed first, followed by the character obtained through indexing.

For example, `"python"` is divided into `"p"` and `"ython"`. The order is then reversed to produce `"ythonp"`.

```python
def rotate_word(text):
    return text[1:] + text[0]

rotate_word(" ")
```

