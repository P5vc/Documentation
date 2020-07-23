# Code Standards

Priveasy puts a lot of pride into the readability and maintainability of its code. However, we also acknowledge that our code isn't necessarily "conventional". We do not stick to any published standards (that we know of) for a variety of reasons, however we are always open to hear you out if you find a standard that you think we should adopt. Feel free to open an issue with any suggestions.

Below you will find a rough outline as to our coding conventions, and specific things we look for when accepting contributions.

## Python

- Always use Python3
- camelCase is better than snake_case
- Variable and functions names should always start with lowercase letters, and classes should always start with capital letters
- Avoid using anything but letters in variable/function/class names whenever practical
- Only comment major blocks of code, or areas were unusual or easily misinterpreted code is used
- Always use single quotes (') instead of double quotes (") around strings
- Space out everything:

Right:

```python
exampleDict = {'Zero' : 0 , 'One' : 1}

if (exampleDict['Zero']):
	print('This should not be printed!')
else:
	randomString = '123Oneabc'
	print(randomString[3 : 6] , ' is equal to:\t' , exampleDict['One'] , sep = '')
```

Wrong:

```python
example_dictionary={"Zero": 0, "One": 1}
if example_dictionary["Zero"]:
    print("This should not be printed!")
else:
    random_string="123Oneabc"
    print(random_string[3:6], " is equal to:\t", example_dictionary["One"], sep="")
```

- Leave two empty lines after/between functions, and three between classes. Use one empty line to separate non-directly-related blocks of code
- Always overuse parentheses to improve readability, and always enclose boolean expressions in parentheses (i.e. in if statements)
- Only expand lists, dictionaries, etc. over multiple lines the first time they are declared, and only if they will be used over and over again and are of some significant length and importance to the code
- We care more about efficiency than readability, but only to a certain extent. Use good judgment when deciding if the efficiency to readability trade-off is worth it, when writing code
- If there's a simple way to write the code without requiring the use of a dependency not built into the python standard library, write it that way... even if it takes up a few more lines or a bit more time to write
- Only import what you need
- Make your lines as long as you need (without being impractical about it)
- Always use tabs instead of spaces
- Never leave trailing spaces/tabs at the end of a line
