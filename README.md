# Relos_ECE2112_PA1
The content of this repository contains Programming Assignment 1 for the course Advance Computer Programming

# **1. Word Rotation Problem**

Create a function named rotate word() that accepts a non-empty string. Move the first character
of the string to the end while keeping all remaining characters in their original order. Preserve the
capitalization of every character

The following function and string operations were used:

• `def rotate_word(text)` - defines the `rotate_word` function, with `text` as its parameter.

• `text[0]` - uses indexing to get the first character.

• `text[1:]` - uses slicing to get the characters after the first character.

For example:

```python
"python"[0]
```

results in:

```text
p
```

while:

```python
"python"[1:]
```

results in:

```text
ython
```

These operations were combined as follows:

```python
def rotate_word(text):
    return text[1:] + text[0]

print(rotate_word("python"))
print(rotate_word("logic"))
print(rotate_word("Code"))
print(rotate_word("A"))
```

The output is:

```text
ythonp
ogicl
odeC
A
```

---

# **2. Username Builder Problem**

Create a function named make username() that accepts two strings: first name and last name. The
function must:
1. convert all letters to lowercase;
2. remove all spaces from the first name;
3. remove all spaces from the last name; and
4. join the processed first and last names using one period (.)

The following function and string methods were used:

• `def make_username(first_name, last_name)` - defines the 'make_username' function with `first_name` and `last_name` as its parameters.

• `.replace(" ", "")` - removes spaces from the names.

• `.lower()` - converts the username to lowercase.

For example:

```python
"Ana Maria".replace(" ", "")
```

results in:

```text
AnaMaria
```

These operations were combined as follows:

```python
def make_username(first_name, last_name):
    return (first_name.replace(" ", "") + "." + last_name.replace(" ", "")).lower()

print(make_username("Ana Maria", "De Leon"))
print(make_username("Ada", "Lovelace"))
print(make_username("Alan", "Turing"))
```

The output is:

```text
anamaria.deleon
ada.lovelace
alan.turing
```

---

# **3. Bookend Swap Problem**

Create a function named `swap_bookends()` that accepts a list containing at least two elements. Unpack the list into three variables:

• `first` – the first element;  
• `middle` – a list containing everything between the first and last elements; and  
• `last` – the last element.

Using these variables, return a new list in which the first and last elements have exchanged positions. The elements in `middle` must remain in their original order. Do not modify the input list.

• `def swap_bookends(items)` - defines the 'swap_bookends' function with `items` as its parameter.

• `first, *middle, last = items` - separates the list into the first element, middle elements, and last element.

• `[last, *middle, first]` - creates a new list with the first and last elements exchanged.

For example:

```python
[1, 2, 3, 4, 5, 6]
```

is unpacked as:

```text
first = 1
middle = [2, 3, 4, 5]
last = 6
```

These operations were combined as follows:

```python
def swap_bookends(items):
    first, *middle, last = items
    return [last, *middle, first]

print(swap_bookends([1, 2, 3, 4, 5, 6]))
print(swap_bookends(["red", "green", "blue"]))
print(swap_bookends([8, 3]))
```

The output is:

```text
[6, 2, 3, 4, 5, 1]
['blue', 'green', 'red']
[3, 8]
```

Thank you for reading!

**README file version history:**
Aug 22 2026 - initial output upload

Aug 25 2026 - content update

Aug 27 2026 - final content update

---
