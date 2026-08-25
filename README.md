# Relos_ECE2112_PA1
The content of this repository contains Programming Assignment 1 for the course Advance Computer Programming

# 1. WORD ROTATION PROBLEM
Create a function named rotate word() that accepts a non-empty string. Move the first character of the string to the end while keeping all remaining characters in their original order. Preserve the capitalization of every character.

The following string operations were applied to solve the problem:
• `text[0]` - uses indexing to access the first character of the string.

Example:

`"python"[0]` --> `"p"`

• `text[1:]` - uses slicing to obtain the characters beginning from the second character up to the end.

Example:

`"python"[1:]` --> `"ython"`

These two parts are then joined together using the `+` operator. The sliced portion is placed first, followed by the character obtained through indexing.

For example, `"python"` is divided into `"p"` and `"ython"`. The order is then reversed to produce `"ythonp"`.

def rotate_word(text):
return text[1:] + text[0]

print(rotate_word("python"))
print(rotate_word("logic"))
print(rotate_word("Code"))
print(rotate_word("A"))
