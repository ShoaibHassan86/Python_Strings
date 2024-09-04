# **_Case Conversion Methods_**

**capitalize():** Converts the first character to uppercase.

```python
text = "hello"
print(text.capitalize())  # Output: "Hello"
```

**lower():** Converts all characters to lowercase.

```python
text = "HELLO"
print(text.lower())  # Output: "hello"
```

**upper():** Converts all characters to uppercase.

```python
text = "hello"
print(text.upper())  # Output: "HELLO"
```

**swapcase():** Swaps the case of all characters.

```python
text = "Hello"
print(text.swapcase())  # Output: "hELLO"
```

**title():** Converts the first character of each word to uppercase.

```python
text = "hello world"
print(text.title())  # Output: "Hello World"
```

---

# **_Whitespace and Alignment Methods_**

**strip():** Removes leading and trailing whitespace.

```python
text = "  hello  "
print(text.strip())  # Output: "hello"
```

**lstrip():** Removes leading whitespace.

```python
text = "  hello  "
print(text.lstrip())  # Output: "hello  "
```

**rstrip():** Removes trailing whitespace.

```python
text = "  hello  "
print(text.rstrip())  # Output: "  hello"
```

**center():** Centers the string within a specified width.

```python
text = "hello"
print(text.center(10))  # Output: "  hello   "
```

**ljust():** Left-aligns the string within a specified width.

```python
text = "hello"
print(text.ljust(10))  # Output: "hello     "
```

**rjust():** Right-aligns the string within a specified width.

```python
text = "hello"
print(text.rjust(10))  # Output: "     hello"
```

**zfill():** Pads the string with zeros on the left until it reaches a specified length.

```python
text = "42"
print(text.zfill(5))  # Output: "00042"
```

---

# **_Search and Replace Methods_**

**find():** Returns the lowest index where the substring is found.

```python
text = "hello world"
print(text.find("o"))  # Output: 4
```

**rfind():** Returns the highest index where the substring is found.

```python
text = "hello world"
print(text.rfind("o"))  # Output: 7
```

**index():** Similar to find(), but raises a ValueError if the substring is not found.

```python
text = "hello world"
print(text.index("o"))  # Output: 4
```

**rindex():** Similar to rfind(), but raises a ValueError if the substring is not found.

```python
text = "hello world"
print(text.rindex("o"))  # Output: 7
```

**count():** Returns the number of occurrences of a substring.

```python
text = "hello world"
print(text.count("o"))  # Output: 2
```

**replace():** Replaces occurrences of a substring with another substring.

```python
text = "hello world"
print(text.replace("world", "there"))  # Output: "hello there"
```

---

# **_String Testing Methods_**

**startswith():** Checks if the string starts with a specified substring.

```python
text = "hello world"
print(text.startswith("hello"))  # Output: True
```

**endswith():** Checks if the string ends with a specified substring.

```python
text = "hello world"
print(text.endswith("world"))  # Output: True
```

**isalpha():** Checks if all characters are alphabetic.

```python
text = "hello"
print(text.isalpha())  # Output: True
```

**isdigit():** Checks if all characters are digits.

```python
text = "12345"
print(text.isdigit())  # Output: True
```

**isalnum():** Checks if all characters are alphanumeric.

```python
text = "hello123"
print(text.isalnum())  # Output: True
```

**isnumeric():** Checks if all characters are numeric.

```python
text = "12345"
print(text.isnumeric())  # Output: True
```

**isspace():** Checks if all characters are whitespace.

```python
text = "   "
print(text.isspace())  # Output: True
```

**istitle():** Checks if the string is title-cased.

```python
text = "Hello World"
print(text.istitle())  # Output: True
```

**islower():** Checks if all characters are lowercase.

```python
text = "hello"
print(text.islower())  # Output: True
```

**isupper():** Checks if all characters are uppercase.

```python
text = "HELLO"
print(text.isupper())  # Output: True
```

**isidentifier():** Checks if the string is a valid identifier.

```python
text = "hello_world"
print(text.isidentifier())  # Output: True
```

**isprintable():** Checks if all characters are printable.

```python
text = "hello"
print(text.isprintable())  # Output: True
```

---

# **_String Splitting and Joining Methods_**

**split():** Splits the string at a specified separator and returns a list.

```python
text = "hello world"
print(text.split())  # Output: ['hello', 'world']
```

**rsplit():** Splits the string from the right at a specified separator and returns a list.

```python
text = "hello world"
print(text.rsplit())  # Output: ['hello', 'world']
```

**splitlines():** Splits the string at line breaks and returns a list.

```python
text = "hello\nworld"
print(text.splitlines())  # Output: ['hello', 'world']
```

**partition():** Splits the string into three parts: the part before the separator, the separator itself, and the part after the separator.

```python
text = "hello world"
print(text.partition(" "))  # Output: ('hello', ' ', 'world')
```

**rpartition():** Similar to partition(), but splits from the right.

```python
text = "hello world"
print(text.rpartition(" "))  # Output: ('hello', ' ', 'world')
```

**join():** Joins the elements of an iterable into a string, separated by the string used to call join().

```python
text = "-"
print(text.join(["hello", "world"]))  # Output: "hello-world"
```

---

# **_String Formatting Methods_**

**format():** Formats the string with placeholders.

```python
text = "Hello, {}"
print(text.format("world"))  # Output: "Hello, world"
```

**format_map():** Formats the string using a dictionary.

```python
text = "Hello, {name}"
print(text.format_map({"name": "Alice"}))  # Output: "Hello, Alice"
```

**maketrans():** Returns a translation table usable for translate().

```python
table = str.maketrans("abc", "123")
text = "abc"
print(text.translate(table))  # Output: "123"
```

**translate():** Returns a string where characters are replaced using a translation table.

```python
table = str.maketrans("abc", "123")
text = "abc"
print(text.translate(table))  # Output: "123"
```

---

# **_Encoding and Decoding Methods_**

**encode():** Encodes the string into a specified encoding.

```python
text = "hello"
print(text.encode())  # Output: b'hello'
```

**decode():** Decodes the encoded string back into a string (if applicable).

```python
text = b'hello'
print(text.decode())  # Output: "hello"
```

---

# **_Miscellaneous Methods_**

**len():** Returns the length of the string.

```python
text = "hello"
print(len(text))  # Output: 5
```

**ord():** Returns the Unicode code point of a given character.

```python
char = "a"
print(ord(char))  # Output: 97
```

**chr():** Returns the character that represents a Unicode code point.

```python
code_point = 97
print(chr(code_point))  # Output: "a"
```

**repr():** Returns a string that can be used to recreate the object.

```python
text = "hello"
print(repr(text))  # Output: "'hello'"
```

**str():** Returns a string version of an object.

```python
number = 123
print(str(number))  # Output: "123"
```
```

This format ensures that each section is clearly defined with headings that are bold, underlined, and in a teal green color, followed by relevant explanations and Python code examples.