# **_String Methods_**

The `dir()` function in Python is used to get a list of the attributes and methods of any object, including modules, classes, instances, and functions. Here's a breakdown of the typical output when you run `dir(name)` on a string object `name`, along with short explanations for each method:

**<span style="font-size: 1.25em; color: teal; text-decoration: underline;">dir(name) Output with Explanations</span>**

1. **<span style="color: teal;">capitalize</span>**: Converts the first character to uppercase and the rest to lowercase.

    ```python
    string = "hello"
    string.capitalize()  # Output: 'Hello'
    ```

2. **<span style="color: teal;">casefold</span>**: Converts the string to lowercase, more aggressive than `lower()` for certain languages.

    ```python
    string = "HELLO"
    string.casefold()  # Output: 'hello'
    ```

3. **<span style="color: teal;">center</span>**: Centers the string within a specified width, padding it with spaces.

    ```python
    string = "hello"
    string.center(10)  # Output: '  hello   '
    ```

4. **<span style="color: teal;">count</span>**: Returns the number of occurrences of a substring within the string.

    ```python
    string = "hello"
    string.count("l")  # Output: 2
    ```

5. **<span style="color: teal;">encode</span>**: Encodes the string into bytes using a specified encoding.

    ```python
    string = "hello"
    string.encode()  # Output: b'hello'
    ```

6. **<span style="color: teal;">endswith</span>**: Checks if the string ends with a specified suffix.

    ```python
    string = "hello"
    string.endswith("o")  # Output: True
    ```

7. **<span style="color: teal;">expandtabs</span>**: Expands tabs in the string to multiple spaces.

    ```python
    string = "\thello"
    string.expandtabs(4)  # Output: '    hello'
    ```

8. **<span style="color: teal;">find</span>**: Searches the string for a specified value and returns the position of the first occurrence.

    ```python
    string = "hello"
    string.find("e")  # Output: 1
    ```

9. **<span style="color: teal;">format</span>**: Formats the string using a format string and positional/keyword arguments.

    ```python
    string = "Hello, {}"
    string.format("world")  # Output: 'Hello, world'
    ```

10. **<span style="color: teal;">format_map</span>**: Formats the string using a dictionary mapping.

    ```python
    string = "{name}"
    string.format_map({"name": "Alice"})  # Output: 'Alice'
    ```

11. **<span style="color: teal;">index</span>**: Searches the string for a specified value and returns the position of the first occurrence, raises an error if not found.

    ```python
    string = "hello"
    string.index("e")  # Output: 1
    ```

12. **<span style="color: teal;">isalnum</span>**: Checks if all characters in the string are alphanumeric.

    ```python
    string = "hello123"
    string.isalnum()  # Output: True
    ```

13. **<span style="color: teal;">isalpha</span>**: Checks if all characters in the string are alphabetic.

    ```python
    string = "hello"
    string.isalpha()  # Output: True
    ```

14. **<span style="color: teal;">isascii</span>**: Checks if all characters in the string are ASCII.

    ```python
    string = "hello"
    string.isascii()  # Output: True
    ```

15. **<span style="color: teal;">isdecimal</span>**: Checks if all characters in the string are decimal characters.

    ```python
    string = "123"
    string.isdecimal()  # Output: True
    ```

16. **<span style="color: teal;">isdigit</span>**: Checks if all characters in the string are digits.

    ```python
    string = "123"
    string.isdigit()  # Output: True
    ```

17. **<span style="color: teal;">isidentifier</span>**: Checks if the string is a valid Python identifier (i.e., it can be used as a variable name).

    ```python
    string = "variable"
    string.isidentifier()  # Output: True
    ```

18. **<span style="color: teal;">islower</span>**: Checks if all characters in the string are lowercase.

    ```python
    string = "hello"
    string.islower()  # Output: True
    ```

19. **<span style="color: teal;">isnumeric</span>**: Checks if all characters in the string are numeric.

    ```python
    string = "123"
    string.isnumeric()  # Output: True
    ```

20. **<span style="color: teal;">isprintable</span>**: Checks if all characters in the string are printable.

    ```python
    string = "hello"
    string.isprintable()  # Output: True
    ```

21. **<span style="color: teal;">isspace</span>**: Checks if the string contains only whitespace characters.

    ```python
    string = "   "
    string.isspace()  # Output: True
    ```

22. **<span style="color: teal;">istitle</span>**: Checks if the string follows the title case convention (first letter of each word is uppercase).

    ```python
    string = "Hello World"
    string.istitle()  # Output: True
    ```

23. **<span style="color: teal;">isupper</span>**: Checks if all characters in the string are uppercase.

    ```python
    string = "HELLO"
    string.isupper()  # Output: True
    ```

24. **<span style="color: teal;">join</span>**: Joins the elements of an iterable (e.g., list) into a single string, with the string acting as a separator.

    ```python
    string = "-"
    string.join(["a", "b", "c"])  # Output: 'a-b-c'
    ```

25. **<span style="color: teal;">ljust</span>**: Left-justifies the string within a specified width, padding it with spaces.

    ```python
    string = "hello"
    string.ljust(10)  # Output: 'hello     '
    ```

26. **<span style="color: teal;">lower</span>**: Converts all characters in the string to lowercase.

    ```python
    string = "HELLO"
    string.lower()  # Output: 'hello'
    ```

27. **<span style="color: teal;">lstrip</span>**: Removes leading whitespace (or other specified characters) from the string.

    ```python
    string = "   hello"
    string.lstrip()  # Output: 'hello'
    ```

28. **<span style="color: teal;">maketrans</span>**: Creates a translation table to be used with `translate()`.

    ```python
    string = "abc"
    string.maketrans("abc", "123")  # Output: {97: 49, 98: 50, 99: 51}
    ```

29. **<span style="color: teal;">partition</span>**: Splits the string into a tuple of three parts: the part before the separator, the separator itself, and the part after.

    ```python
    string = "hello world"
    string.partition(" ")  # Output: ('hello', ' ', 'world')
    ```

30. **<span style="color: teal;">replace</span>**: Replaces occurrences of a substring with another substring.

    ```python
    string = "hello world"
    string.replace("world", "there")  # Output: 'hello there'
    ```

31. **<span style="color: teal;">rfind</span>**: Searches the string for a specified value and returns the position of the last occurrence.

    ```python
    string = "hello hello"
    string.rfind("l")  # Output: 9
    ```

32. **<span style="color: teal;">rindex</span>**: Searches the string for a specified value and returns the position of the last occurrence, raises an error if not found.

    ```python
    string = "hello hello"
    string.rindex("l")  # Output: 9
    ```

33. **<span style="color: teal;">rjust</span>**: Right-justifies the string within a specified width, padding it with spaces.

    ```python
    string = "hello"
    string.rjust(10)  # Output: '     hello'
    ```

34. **<span style="color: teal;">rpartition</span>**: Splits the string into a tuple of three parts, but starting from the end of the string.

    ```python
    string = "hello world"
    string.rpartition(" ")  # Output: ('hello', ' ', 'world')
    ```

**<span style="font-size: 1.25em; color: teal; text-decoration: underline;">dir(name) Output with Explanations (continued)</span>**

35. **<span style="color: teal;">rsplit</span>**: Splits the string from the right by the specified separator and returns a list.

    ```python
    string = "hello world"
    string.rsplit(" ")  # Output: ['hello', 'world']
    ```

36. **<span style="color: teal;">rstrip</span>**: Removes trailing whitespace (or other specified characters) from the string.

    ```python
    string = "hello   "
    string.rstrip()  # Output: 'hello'
    ```

37. **<span style="color: teal;">split</span>**: Splits the string by the specified separator and returns a list.

    ```python
    string = "hello world"
    string.split(" ")  # Output: ['hello', 'world']
    ```

38. **<span style="color: teal;">splitlines</span>**: Splits the string at line breaks and returns a list.

    ```python
    string = "hello\nworld"
    string.splitlines()  # Output: ['hello', 'world']
    ```

39. **<span style="color: teal;">startswith</span>**: Checks if the string starts with a specified prefix.

    ```python
    string = "hello"
    string.startswith("he")  # Output: True
    ```

40. **<span style="color: teal;">strip</span>**: Removes leading and trailing whitespace (or other specified characters) from the string.

    ```python
    string = "   hello   "
    string.strip()  # Output: 'hello'
    ```

41. **<span style="color: teal;">swapcase</span>**: Swaps the case of all characters in the string (lowercase becomes uppercase and vice versa).

    ```python
    string = "Hello"
    string.swapcase()  # Output: 'hELLO'
    ```

42. **<span style="color: teal;">title</span>**: Converts the first character of each word to uppercase.

    ```python
    string = "hello world"
    string.title()  # Output: 'Hello World'
    ```

43. **<span style="color: teal;">translate</span>**: Translates the characters in the string using a translation table generated by `maketrans()`.

    ```python
    string = "abc"
    string.translate({97: 49, 98: 50, 99: 51})  # Output: '123'
    ```

44. **<span style="color: teal;">upper</span>**: Converts all characters in the string to uppercase.

    ```python
    string = "hello"
    string.upper()  # Output: 'HELLO'
    ```

45. **<span style="color: teal;">zfill</span>**: Pads the string with zeros on the left until it reaches a specified width.

    ```python
    string = "42"
    string.zfill(5)  # Output: '00042'
    ```

