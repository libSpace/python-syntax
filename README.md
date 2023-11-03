# Python-Syntax

## Table of Contents

- [Intro to Python](#Intro-to-Python)
- [Variables](#Variables)
- [Data Types](#Data-Types)
- [Operators](#Operators)


## Intro-to-Python


History of Python
•	Python is a popular programming language. It was created by Guido van Rossum and released in 1991.
•	Python strikes a good balance between fast compilations and readability.

Python Indentation
•	Indentation in Python identifies what code belongs to what section of code.
•	Indentation refers to the spaces at the beginning of a code line.
if 5 > 2:
  print("Five is greater than two!")
•	Python will give you an error if you skip the indentation:
if 5 > 2:
print("Five is greater than two!")


Comments in Python
In programming, comments are a programming language construct used to insert human-readable text in the source code of a program.
•	Comments are added to make the source code easier to understand.
Comments could be used for a wide range of purposes, for example: 
•	Augmenting program code with basic descriptions to generate external documentation.
•	Integration with source code management systems and other kinds of external programming tools.

•	Comments in Python start with the hash character, #, and extend to the end of the physical line.
•	A comment may appear at the start of a line or following whitespace or code, but not within a string literal.
•	Commenting has its advantages: for example, if a programmer creates an application and there are bugs in the code, another programmer can easily follow what the first programmer has done by reading the comments, which means the problematic code is found more easily and can be fixed faster.

Escape Sequences
 Description
 Token  
Backslash character (\)
 \\
New line feed
\n 
Tab
\t 
Vertical tab
\v 
Backspace
\b
Carriage return
\r
Single quote (useful in strings enclosed in single quotes: ‘hello \ ‘World’)
\' 
Double quote (useful in strings enclosed in single quotes: “hello \ “World”)
•	\"
•	If you do not want to use the \n escape sequence, you can use three single quotes ‘’’ or three double quotes “""characters.


## Variables


Python Variables
•	Variables are a temporary storage space in a computer’s memory.
•	Variables are containers for storing data values.

A variable can be in three states:
•	Variable creation (Declaration)
•	Variable assignment (Initialization)
•	Variable changed (Execution)

•	In Python, variables are defined in a standard way, by using the assignment character (=).
•	Variable names may contain any upper or lower case letter (A–Z, a–z), a number, or the underscore character. 
•	They may not begin with a number or contain spaces.

There are several techniques you can use to make them more readable:
Camel Case
Each word, except the first, starts with a capital letter:
myVariableName = "John"
________________________________________
Pascal Case
Each word starts with a capital letter:
MyVariableName = "John"
________________________________________
Snake Case
Each word is separated by an underscore character:
my_variable_name = "John"


Here are a few examples of valid variable names:
•	c
•	ref_number
•	admin
•	aVeryLongName

Here are a few examples of invalid variable names:
•	True
•	$name
•	12Graph

•	In Python identifiers are case sensitive, so for example, firstName, FirstName, FIRSTNAME, and firstname are four different identifiers.
•	A second rule is that variables cannot have the same name as Python’s keywords.

•	If this function is called with the __builtins__ attribute, it returns a list of Python’s built-in attributes.
•	The __builtins__ module contains all Python’s built-in attributes, which can be used with the dir()function.

The ones that are returned are identified with the following characteristics:
•	Python’s built-in exceptions start with a capital letter.
•	The rest are either functions or data type names.
•	Identifiers that start and end with one or two underscores are special methods.

 NOTE
 All of the methods, exceptions, and functions contained in  
dir(__builtins__), dir(__doc__), dir(__name__), and dir(__package__) cannot be used as variable names.

Python has a set of keywords that are reserved words that cannot be used as variable names, function names, or any other identifiers:
Keyword	Description
and
A logical operator
as
To create an alias
assert
For debugging
break
To break out of a loop
class
To define a class
continue
To continue to the next iteration of a loop
def
To define a function
del
To delete an object
elif
Used in conditional statements, same as else if
else
Used in conditional statements
except
Used with exceptions, what to do when an exception occurs
False
Boolean value, result of comparison operations
finally
Used with exceptions, a block of code that will be executed no matter if there is an exception or not
for
To create a for loop
from
To import specific parts of a module
global
To declare a global variable
if
To make a conditional statement
import
To import a module
in
To check if a value is present in a list, tuple, etc.
is
To test if two variables are equal
lambda
To create an anonymous function
None
Represents a null value
nonlocal
To declare a non-local variable
not
A logical operator
or
A logical operator
pass
A null statement, a statement that will do nothing
raise
To raise an exception
return
To exit a function and return a value
True
Boolean value, result of comparison operations
try
To make a try...except statement
while
To create a while loop
with	Used to simplify exception handling
yield	To end a function, returns a generator


Using variables
All variables must be assigned to a data type like a string (a series of characters) or an integer (positive and negative whole numbers).
•	Python automatically assigns a variable to a string data-type, if an input or value is given that contains letters or words.

•	To create a global variable inside a function, you can use the global keyword.


Casting
If you want to specify the data type of a variable, this can be done with casting.

Casting can be done in two ways:
•	Implicitly: The compiler automatically casts a value from one data type to another when assured that there will be no data loss.
For example. casting from an integer variable to a floating-point variable or casting from an integer variable to another integer variable 
•	Explicitly: A value cannot be automatically cast from one data type to another if it will result in data loss. Extra code has to be written to ensure that the value stays the same and only the data type changes.
For example, casting from a floating-point value to an integer value.

## Data-Types



Data types covered in this course include:
 Data Types
 Examples
 Integers
 These represent numbers in an unlimited range. This is only limited by a machine’s memory.

 Booleans
 Evaluate to ‘True or False’, 1 or 0 respectively.

 Floating point numbers
 Floating-point numbers represent double-precision numbers.

 Complex numbers
 Complex numbers represent numbers as a pair of double-precision numbers.

 Strings
 A sequence of Unicode characters e.g. a word or a sentence that can be manipulated.

Literals are an alternative to using variables. Examples of literals include:
•	"This is only a string"
•	"\t"
•	2
Python has the following data types built-in by default, in these categories:
Text Type:	str
Numeric Types:	int, float, complex
Sequence Types:	list, tuple, range
Mapping Type:	dict
Set Types:	set, frozenset
Boolean Type:	bool
Binary Types:	bytes, bytearray, memoryview
None Type:	NoneType
Manipulate Booleans
 Syntax
 Description
 a or b
 
If either a or b is True, then the result will be True. 
If both a and b are False then the result will be False.
 a and b
 If a and b are True, then the result will be True. Otherwise, the result will be False.
 not a
 If a is True, False is returned. If a is False, True is returned.

•	Float can also be scientific numbers with an "e" to indicate the power of 10.
Floats:
x = 35e3
y = 12E4
z = -87.7e100

print(type(x))
print(type(y))
print(type(z))


Complex
Complex numbers are written with a "j" as the imaginary part:
Example
Complex:
x = 3+5j
y = 5j
z = -5j

print(type(x))
print(type(y))
print(type(z))


Getting the Data Type
You can get the data type of any object by using the type() function:
x = 5
print(type(x))

Lambda Expressions
•	This function returns the sum of its two arguments: lambda a, b: a+b.
•	Lambda functions can be used wherever function objects are required.
•	hey are syntactically restricted to a single expression.
•	A lambda function is a small anonymous function.
•	A lambda function can take any number of arguments, but can only have one expression.
Add 10 to argument a, and return the result:
x = lambda a : a + 10
print(x(5))


## Operators


•	Operators are used to perform operations on variables and values.
•	Operators are used to testing conditions and manipulating values.
•	When two objects of a different type, like str and int, are compared they are never equal, except for different numeric types like int and float which can be equal.

•	List is a collection which is ordered and changeable. Allows duplicate members.
•	Tuple is a collection which is ordered and unchangeable. Allows duplicate members.
•	Set is a collection which is unordered, unchangeable*, and unindexed. No duplicate members.
•	Dictionary is a collection which is ordered** and changeable. No duplicate members.
I Embrace the journey of growth, it is the path to unlocking my fullest potential. Every challenge I face is an opportunity to learn, adapt, and evolve. As I step out of my comfort zone, I remember that discomfort is often the precursor to progress. I Believe in my capacity to overcome obstacles and thrive. With each new experience, I’m sculpting a stronger, wiser version of yourself.
