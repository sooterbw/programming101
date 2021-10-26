# programming101
This is a quick overview of programming basics

## Data Types
- String
- Integer
- Float
- Boolean
- Null

## Variables
Variables are used to store data.
### Naming Conventions
- camelCase
- snake_case
- PascalCase
- CONSTANT_VARIABLE

Variable names should always be descriptive.
The farther removed a variable is from its' use, the more descriptive it should be.

## Functions

Javascript
```javascript
function test(name) {
 console.log(`Hello ${name}!`);
}

// test("Bob");
// out: "Hello Bob!"
```

Python
```python
def test(name) {
 print(f"Hello {name}!");
}

# test("Bob")
# out: "Hello Bob!"
```

The anatomy of a function remains generally consistent regardless of which language you use.

In Both examples we created our function with the following components:
1. We defined that it is a function:
  - ```function``` in Javascript
  - ```def``` in Python

2. Then the function is named. ```test```.
3. We then pass in what arguments our function needs to take. ```name```
4. Finally we output the result to the command line using built in functions.
  - ```console.log()``` in JavaScript
  - ```print()``` in Python

Note that our function does not contain a ```return``` statement.

If we were to attempt to store our function ```test()``` in a variable it would return ```undefined```.

In this example we will create a function that adds two numbers together and returns the value to be used later.

```python
def add(num_one, num_two):
  return num_one + num_two
```

Now, if we want, we can take our function and store the result in a variable.
```python
my_variable = add(2,2) # 4
```

### When to use a function
Use the DRY method. Don't Repeat Yourself. If you find there is a block of code that you will need to reuse later, make it a function.

## Lists / Arrays
Lists (commonly referred to as arrays) is data seperated by commas typically encapsulated by brackets.
```python
my_list = [1,2,3,4]
```

```my_list``` conatins a list made up of integers.

Lists can contain any type of data and can be mixed with other types (although this isn't typically reccomended).

```python
my_new_list = [1, "a", True, 3.14]
```

```my_new_list``` contains a list made up of an int, string, bool, and float.

### Grabbing a value from a list
If we would like to retrieve a value from a stored list, all we have to do is put the position of the value we would like to grab in brackets at the end of the variable.

Remember, counting starts at 0.
```python
my_list = [1,2,3,4]

my_list[0] # 1
my_list[1] # 2
my_list[2] # 3
my_list[3] # 4
my_list[4] # IndexError: list index out of range
```

## Conditions and Operators
Condition statements are statements that return a boolean value.
- ```==``` Is equal to
- ```!=``` Is not equal to
- ```<``` Less than
- ```<=``` Less than or equal to
- ```>``` Greater than
- ```>=``` Greater than or equal to

```python
1 == 1 # True
1 == "1" # False
1 >= 1 # True
```

Operators tie multiple conditions together. The most common being ```and``` (```&&```) or ```or``` (```||```).

``or`` means at least one of the conditional statements are true
```python
1 == 1 or 0 == 1 # True
1 >= 2 or 0 > 1 # False
```

``and`` requires that both conditional statements are true
```python
1 == 1 and 0 == 1 # False
```

## If Statements
Simply: If this, do that

If statements are one of the simplist logical
