# Python Quickstart

Python is an interpreted programming language, which means that as a developer, you write Python (.py) files in a text editor and then put those files into the Python interpreter to be executed.

To run a Python file from the command line, use the following syntax:

```bash
C:\Users\Your Name>python helloworld.py
```

Here, "helloworld.py" is the name of your Python file.

Let's write our first Python file, called helloworld.py, in any text editor:

helloworld.py

```python

print("Hello, World!")

```

Save your file. Then open your command line, navigate to the directory where you saved your file, and run:

```bash

C:\Users\Your Name>python helloworld.py
```

The output should read:

```bash

Hello, World!
```

Congratulations! You have written and executed your first Python program.

Python Version
To check the Python version, you can import the sys module and print the version:

```python

import sys


print(sys.version)
```

You will learn more about importing modules in our Python Modules chapter.

The Python Command Line
To test a short amount of code in Python, sometimes it's quickest and easiest not to write the code in a file. Python can be run as a command line itself.

Type the following on the Windows, Mac, or Linux command line:

```bash

C:\Users\Your Name>python

Or, if the "python" command did not work, you can try "py":
```

```bash

C:\Users\Your Name>py
```

From there, you can write any Python code, including our hello world example:

```python

print("Hello, World!")
```

Which will output "Hello, World!" in the command line.

Whenever you are done in the Python command line, you can simply type the following to quit:

```bash

exit()
```

### Here are some key notes summarizing Python's essential features and concepts:

- Interpreted Language: Python is an interpreted language, meaning that code is executed line by line by an interpreter.

- Dynamic Typing: Python uses dynamic typing, allowing variables to change types during execution.

- Indentation: Python uses indentation to define blocks of code, such as loops, functions, and conditional statements.

- Object-Oriented: Python supports object-oriented programming (OOP) paradigms, including classes, objects, inheritance, and polymorphism.

- Simple and Readable Syntax: Python's syntax is designed to be straightforward and readable, with clear, concise code.

- Extensive Standard Library: Python comes with a large standard library that provides modules and functions for various tasks, reducing the need for external dependencies.

- Cross-platform: Python is available on multiple platforms, including Windows, macOS, and Linux, ensuring code portability.

- High-level Language: Python abstracts many low-level details, enabling developers to focus on problem-solving rather than system complexities.

- Large Ecosystem: Python has a vast ecosystem of third-party libraries and frameworks for various domains, such as web development, data science, and machine learning.

- Community Support: Python has a large and active community of developers who contribute to its development, provide support, and create resources for learning and collaboration.

- Open Source: Python is developed under an open-source license, allowing users to freely use, modify, and distribute the language and its implementations.

- Multiparadigm: Python supports multiple programming paradigms, including procedural, functional, and imperative programming styles.

- Exception Handling: Python provides robust mechanisms for handling exceptions, allowing developers to gracefully manage errors in their code.

- Documentation: Python emphasizes the importance of clear and comprehensive documentation, ensuring that users can easily understand and utilize its features and functionalities.

- Versatility: Python is a versatile language suitable for various applications, including web development, automation, scientific computing, data analysis, artificial intelligence, and more.

# Python Syntax

## Execute Python Syntax

As we learned in the previous page, Python syntax can be executed by writing directly in the Command Line:

```python
>>> print("Hello, World!")
Hello, World!
```

Or by creating a python file on the server, using the .py file extension, and running it in the Command Line:

```
C:\Users\Your Name>python myfile.py

```

# Python Indentation

Indentation refers to the spaces at the beginning of a code line.

In Python, indentation is very important as it is used to indicate a block of code. Unlike other programming languages where indentation is for readability only, in Python, it is a part of the syntax and affects how the code is executed.

## Example

```python
if 5 > 2:
    print("Five is greater than two!")

```

Python will give you an error if you skip the indentation:

```python
# Syntax Error:
if 5 > 2:
print("Five is greater than two!")
```

The number of spaces is up to you as a programmer, the most common use is four, but it has to be at least one.

```python
# Examples
if 5 > 2:
    print("Five is greater than two!")
if 5 > 2:
        print("Five is greater than two!")

```

You have to use the same number of spaces in the same block of code, otherwise Python will give you an error:

```python
# Syntax Error:
if 5 > 2:
    print("Five is greater than two!")
        print("Five is greater than two!")

```

# Python Variables

In Python, variables are created when you assign a value to them. Unlike some other programming languages, Python has no command for declaring a variable.

## Example

```python
# Variables in Python:
x = 5
y = "Hello, World!"
```

Here, x is assigned the integer value 5, and y is assigned the string value "Hello, World!".

### Learning More

You will learn more about variables in the Python Variables chapter, including different data types, variable naming conventions, and variable scope.

# Python Comments

Comments can be used to explain Python code.

Comments can be used to make the code more readable.

Comments can be used to prevent execution when testing code.

## Creating a Comment

Comments start with a `#`, and Python will ignore them:

```python
# This is a comment
print("Hello, World!")
```

Comments can be placed at the end of a line, and Python will ignore the rest of the line:
```python
print("Hello, World!")  # This is a comment
```
A comment does not have to be text that explains the code; it can also be used to prevent Python from executing code:
```python
# print("Hello, World!")
print("Cheers, Mate!")
```
## Multiline Comments
Python does not really have a syntax for multiline comments.

To add a multiline comment, you could insert a # for each line:
```python
# This is a comment
# written in
# more than just one line
print("Hello, World!")
```
Or, not quite as intended, you can use a multiline string.

Since Python will ignore string literals that are not assigned to a variable, you can add a multiline string (triple quotes) in your code, and place your comment inside it:

```python
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")
```


## Best Practices

- Be Clear and Concise: Write comments that are easy to understand and provide valuable information to readers.
- Update Comments: Keep comments up-to-date with the code. If code changes, update corresponding comments.
- Avoid Over-commenting: While comments are helpful, excessive comments can clutter code and reduce readability. Focus on commenting where necessary.
- Use Comments Sparingly: Write code that is self-explanatory whenever possible, minimizing the need for comments.
- Comments are an essential aspect of good coding practices, helping to improve code readability and maintainability.

# Conclusion

Python is a versatile and powerful programming language with a simple and readable syntax. Whether you're a beginner or an experienced developer, Python offers a wide range of capabilities for various applications, including web development, data analysis, artificial intelligence, scientific computing, and more.

In this guide, we've covered some fundamental aspects of Python programming, including its syntax, indentation, variables, and comments. We've also provided examples and best practices to help you understand how to write clean and effective Python code.

As you continue your journey with Python, remember to explore the vast ecosystem of libraries, frameworks, and resources available to enhance your development experience. Additionally, practice writing code, engage with the Python community, and keep learning to sharpen your skills and become proficient in Python programming.

With its simplicity, flexibility, and extensive capabilities, Python is an excellent choice for anyone looking to dive into the world of programming and build exciting projects.

Happy coding! ## Digiview Training Institude
