
# **Python String Methods**

### __1. Case Conversion__  
These methods are used to change the case of the string.

- `str.upper()`
  ```python
  text = "hello world"
  print(text.upper())  # Output: "HELLO WORLD"
  ```

- `str.lower()`
  ```python
  text = "HELLO WORLD"
  print(text.lower())  # Output: "hello world"
  ```

- `str.capitalize()`
  ```python
  text = "hello world"
  print(text.capitalize())  # Output: "Hello world"
  ```

- `str.title()`
  ```python
  text = "hello world"
  print(text.title())  # Output: "Hello World"
  ```

- `str.swapcase()`
  ```python
  text = "Hello World"
  print(text.swapcase())  # Output: "hELLO wORLD"
  ```

### __2. Trimming & Padding__  
These methods are used to remove spaces or add padding to the string.

- `str.strip([chars])`
  ```python
  text = "   hello   "
  print(text.strip())  # Output: "hello"
  ```

- `str.lstrip([chars])`
  ```python
  text = "   hello   "
  print(text.lstrip())  # Output: "hello   "
  ```

- `str.rstrip([chars])`
  ```python
  text = "   hello   "
  print(text.rstrip())  # Output: "   hello"
  ```

- `str.zfill(width)`
  ```python
  text = "42"
  print(text.zfill(5))  # Output: "00042"
  ```

- `str.center(width[, fillchar])`
  ```python
  text = "hello"
  print(text.center(10, "-"))  # Output: "--hello---"
  ```

- `str.ljust(width[, fillchar])`
  ```python
  text = "hello"
  print(text.ljust(10, "-"))  # Output: "hello-----"
  ```

- `str.rjust(width[, fillchar])`
  ```python
  text = "hello"
  print(text.rjust(10, "-"))  # Output: "-----hello"
  ```

### __3. Search & Replace__  
These methods are used to search for substrings or replace them.

- `str.find(sub[, start[, end]])`
  ```python
  text = "hello world"
  print(text.find("world"))  # Output: 6
  ```

- `str.rfind(sub[, start[, end]])`
  ```python
  text = "hello world world"
  print(text.rfind("world"))  # Output: 12
  ```

- `str.index(sub[, start[, end]])`
  ```python
  text = "hello world"
  print(text.index("world"))  # Output: 6
  ```

- `str.rindex(sub[, start[, end]])`
  ```python
  text = "hello world world"
  print(text.rindex("world"))  # Output: 12
  ```

- `str.replace(old, new[, count])`
  ```python
  text = "hello world"
  print(text.replace("world", "Python"))  # Output: "hello Python"
  ```

- `str.count(sub[, start[, end]])`
  ```python
  text = "hello world world"
  print(text.count("world"))  # Output: 2
  ```

### __4. Check Types__  
These methods are used to check the properties of the string.

- `str.isalnum()`
  ```python
  text = "hello123"
  print(text.isalnum())  # Output: True
  ```

- `str.isalpha()`
  ```python
  text = "hello"
  print(text.isalpha())  # Output: True
  ```

- `str.isdigit()`
  ```python
  text = "12345"
  print(text.isdigit())  # Output: True
  ```

- `str.islower()`
  ```python
  text = "hello"
  print(text.islower())  # Output: True
  ```

- `str.isupper()`
  ```python
  text = "HELLO"
  print(text.isupper())  # Output: True
  ```

- `str.isspace()`
  ```python
  text = "   "
  print(text.isspace())  # Output: True
  ```

- `str.istitle()`
  ```python
  text = "Hello World"
  print(text.istitle())  # Output: True
  ```

### __5. Splitting & Joining__  
These methods are used to split or join strings.

- `str.split(sep=None, maxsplit=-1)`
  ```python
  text = "hello world"
  print(text.split())  # Output: ['hello', 'world']
  ```

- `str.rsplit(sep=None, maxsplit=-1)`
  ```python
  text = "hello world python"
  print(text.rsplit(maxsplit=1))  # Output: ['hello world', 'python']
  ```

- `str.splitlines([keepends])`
  ```python
  text = "hello\nworld"
  print(text.splitlines())  # Output: ['hello', 'world']
  ```

- `str.partition(sep)`
  ```python
  text = "hello world"
  print(text.partition(" "))  # Output: ('hello', ' ', 'world')
  ```

- `str.rpartition(sep)`
  ```python
  text = "hello world python"
  print(text.rpartition(" "))  # Output: ('hello world', ' ', 'python')
  ```

- `str.join(iterable)`
  ```python
  words = ['hello', 'world']
  print(" ".join(words))  # Output: "hello world"
  ```

### __6. Encoding & Decoding__  
These methods are used for encoding and decoding strings.

- `str.encode(encoding="utf-8", errors="strict")`
  ```python
  text = "hello"
  print(text.encode())  # Output: b'hello'
  ```

- `str.decode(encoding="utf-8", errors="strict")`
  ```python
  byte_text = b'hello'
  print(byte_text.decode())  # Output: "hello"
  ```

### __7. Miscellaneous__  
Other useful methods.

- `str.format(*args, **kwargs)`
  ```python
  text = "Hello, {}!"
  print(text.format("world"))  # Output: "Hello, world!"
  ```

- `str.format_map(mapping)`
  ```python
  text = "Hello, {name}!"
  print(text.format_map({"name": "world"}))  # Output: "Hello, world!"
  ```

- `str.expandtabs(tabsize=8)`
  ```python
  text = "hello\tworld"
  print(text.expandtabs(4))  # Output: "hello   world"
  ```

- `str.translate(table)`
  ```python
  text = "hello"
  translation_table = str.maketrans("h", "H")
  print(text.translate(translation_table))  # Output: "Hello"
  ```

- `str.maketrans(x[, y[, z]])`
  ```python
  translation_table = str.maketrans("aeiou", "12345")
  text = "hello world"
  print(text.translate(translation_table))  # Output: "h2ll4 w4rld"
  ```

- `str.casefold()`
  ```python
  text = "Hello World"
  print(text.casefold())  # Output: "hello world"
  ```

- `str.isdecimal()`
  ```python
  text = "12345"
  print(text.isdecimal())  # Output: True
  ```

- `str.isnumeric()`
  ```python
  text = "12345"
  print(text.isnumeric())  # Output: True
  ```

- `str.isidentifier()`
  ```python
  text = "variable1"
  print(text.isidentifier())  # Output: True
  ```
```

### Notes:

1. In VS Code, markdown headings (`#`, `##`, etc.) are rendered slightly larger automatically. To get a teal green color in VS Code markdown, you would typically use a custom theme or settings in your editor.
2. If you'd like to achieve color directly in the markdown file, you'll need to extend VS Code using extensions like "Markdown+Math" or others that support colored text.