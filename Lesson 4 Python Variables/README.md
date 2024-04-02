# Python Variables

## Variables

Variables are containers for storing data values.

### Creating Variables

Python has no command for declaring a variable.

A variable is created the moment you first assign a value to it.

```python
x = 5
y = "John"
print(x)
print(y)
```

Variables do not need to be declared with any particular type, and can even change type after they have been set.

```python
x = 4       # x is of type int
x = "Sally" # x is now of type str
print(x)
```

## Casting

If you want to specify the data type of a variable, this can be done with casting.

```python
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0
```

## Get the Type

You can get the data type of a variable with the type() function.

```python
x = 5
y = "John"
print(type(x))
print(type(y))
```

You will learn more about data types and casting later in this repo.

## Single or Double Quotes?

String variables can be declared either by using single or double quotes:

```python
x = "John"
# is the same as
x = 'John'
```

## Case-Sensitive

Variable names are case-sensitive.

```python
# This will create two variables:
a = 4
A = "Sally"
# A will not overwrite a
```

# Python - Variable Names

## Variable Names

A variable can have a short name (like `x` and `y`) or a more descriptive name (`age`, `carname`, `total_volume`).

### Rules for Python variables:

- A variable name must start with a letter or the underscore character.
- A variable name cannot start with a number.
- A variable name can only contain alpha-numeric characters and underscores (`A-z`, `0-9`, and `_`).
- Variable names are case-sensitive (`age`, `Age`, and `AGE` are three different variables).
- A variable name cannot be any of the Python keywords.

### Example

Legal variable names:

```python
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"

```

