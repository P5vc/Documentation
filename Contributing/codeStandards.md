# Code Standards

Priveasy puts a lot of pride into the readability and maintainability of its code. However, we also acknowledge that our code isn't necessarily "conventional". We do not stick to any published standards (that we know of) for a variety of reasons, however we are always open to hear you out if you find a standard that you think we should adopt. Feel free to open an issue with any suggestions.

Below you will find a rough outline as to our coding conventions, and specific things we look for when accepting contributions.

## Python

### General Rules

- Use Python3
- Only comment when:
  - You're describing the function of a major block of code (docstrings are a valid alternative)
  - You're explaining the function of a particularly unusual or hard-to-read piece of code
  - You have specific intentions that you fear future developers may miss or overlook
- Never unpack lists or dictionaries over multiple lines, unless the following apply:
  - The object is to be referenced many times, and it is of significant importance that a programmer be knowledgeable of it
  - It is the initial declaration of the object
    - The declaration must be made in a separate, proceeding block, even if doing so is redundant
- Care more about efficiency than readability, but only when a valid, noticeable impact would be made, or could be foreseeably made in the future. Use good judgment when deciding if the efficiency to readability trade-off is worth it
- Avoid dependencies whenever reasonable; if you must rely on a dependency, only import what you need
- Do not worry about line length

### Naming Conventions

- Use camelCase over snake_case
- Start variable and function names with lowercase letters
- Start class names with uppercase letters
- Names should only contain letters, whenever practical

### Punctuation

- Always use single quotes (') instead of double quotes (")
- Overuse parentheses to increase readability, with:
  - Mathematical expressions involving two or more operations
  - Conditionals
  - String concatenation

### Spacing

- Use hard tabs for indenting, never spaces
- Leave a space between the octothorpe (#) and the start of the comment
- Never leave any trailing spaces or tabs at the end of a line of code
- Maintain a space between keywords, separators, and variables
- Code blocking:
  - Leave one newline between blocks of code that are not directly related to one another
  - Leave two newlines between separate functions
  - Leave three newlines between separate classes

Wrong:

```python
example_dictionary={"Zero": 0, "One": 1}
if example_dictionary["Zero"]:
    print("This should not be printed!")
else:
    random_string="123Oneabc"
    print(random_string[3:6], " is equal to:\t", example_dictionary["One"], sep="")
```

Right:

```python
exampleDict = {'Zero' : 0 , 'One' : 1}

if (exampleDict['Zero']):
	print('This should not be printed!')
else:
	randomString = '123Oneabc'
	print(randomString[3 : 6] , ' is equal to:\t' , exampleDict['One'] , sep = '')
```
