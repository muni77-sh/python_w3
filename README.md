# python_w3
python course
=================================
1.1.python variable
variables are containers for storing data values.

A varible is created the moment you first assign a value to it.
ex.1
x = 5
y = "John"
print(x)
print(y)

Variables do not need to be declared with any particular type,
 and can even change type after they have been set
ex 
x = 4       # x is of type int
x = "Sally" # x is now of type str
print(x)

*.casting :
if you want to specify the data type of a varibale, this can be done with casting.
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0

get the type:
the data type of a varable with the type() function
x = 5
y = "John"
print(type(x))
print(type(y))
=======================================================================
1.1.Variabe Names:
A variable can have a short (like x and y) or a more descriptive name
(age, carname, total_volume)
rule python variable
--> A variable name must start with a letter or the underscore character
--> A variable name cannot start with a number.
--> A variable name can only contain alpha-numeric character and underscore
(A-Z, 0-9, and_)
--> A variable names are case-sensitive (age, Age and AGE are three dfferent variables)

myvar = "john"
my_var = "john"
_my_var = "john"
myVar = "john"
MYVAR = "john"
myvar2 = "john"

print(myvar)
print(my_var)
print(_my_var)
print(myVar)
print(MYVAR)
print(myvar2)

*. multi words variabe names
variable names with more than one word can be dfficult to read.
there are several techniques you can use to make them more readable.

-->camel case
each word, except the first, starts with a capital letter:
myVarableName = "john"

--> pascal case
each word starts with a capital letter
MyvariableName = "john"

-->snake case
each word is separated by an underscore character:
my_variable_name = "john"
================================================
1.2 many values to multipe variable
python allows you to assign to multipe variable in one line:

x, y, z = "orange", "banana", "mango"
print(x)
print(y)
print(z)

*. One value to multiple variables
you can assign the same value to multiple variables in one line:
x = y = z = "orange"
print(x)
print(y)
print(z)

*. unpack a collectio:
python allows you extract the values into variable.
this called unpacking.

fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)
===================================================
1.2. output variable
the python print statement is often used to output variables.

to combine both text and a variable, python uses the + character:

x = "awesome"
print("python is " + x)

*.you can also the + character to add a variable to another variable
x = "python is "
y = "awesome"
z = x + y
print(z)

x = "python is "
y = "awesome"
z = x + y
print(z)
* number the + character works as a mathematical oper
x = 5
y = 10
print(x + y)
=============================================================
 1.3
Global variables:
Variable that are created of a function (as in all of the example above) are known as global varibales.
Global variables can be used by everyone, both inside of functions and outside.

x = "awesome"

def myfunc():
   print("python is " + x)
   myfunc()

if you create a variable with same name inside a function, this variable will be local and
can only be used inside the function. The global variable with the same will remain as it was,
global and with the original value.

create a variable inside a function, with same as the global veriable

*. the Global keyword
Normally, when you create a variable inside a function, that variable is local,
and can only be used inside that function.
to create a global variable inside a function, you can use the global keyword.

def myfunc():
    global x
    x = "fantastic"

    myfunc()

    print("python is " + x)

use the global keyword if you want to change a global variable inside a function


def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
=============================================================================

2. Data types:
setting the data type:

variables can store data of different types, and different types can do different things
data types built-in by default

Text Type:	str
Numeric Types:	int, float, complex
Sequence Types:	list, tuple, range
Mapping Type:	dict
Set Types:	set, frozenset
Boolean Type:	bool
Binary Types:	bytes, bytearray, memoryview

*. ex print data of the variable x:
x = 5
 print(type(x))

1.a
data type(str)
x = "Hello World"

#display x:
print(x)

#display the data type of x:
print(type(x))

1.b
data type(int)
x = 20

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.c
data type(float)
x = 20.5

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.d
data type(complex)
x = 1j

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.e
data type(list)
x = ["apple", "banana", "cherry"]

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.f
data type(tuple)
x = ("apple", "banana", "cherry")

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.g
data type(range)
x = range(6)

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.h
data type(dict)
x = {"name" : "John", "age" : 36}

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.j
data type(set)
x = {"apple", "banana", "cherry"}

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.k
data type(frozenset)
x = frozenset({"apple", "banana", "cherry"})

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.L
data type(bool)
x = True

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.M
data ype(bytes)
x = b"Hello"

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.N
data type(bytearray)
x = bytearray(5)

#display x:
print(x)

#display the data type of x:
print(type(x)) 

1.O
data type(memoryview)
x = memoryview(bytes(5))

#display x:
print(x)

#display the data type of x:
print(type(x)) 


=======================================================================
2.1
setting the specific Datatype:

2.11
data type(str)
x = str("Hello World")

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.12
data type(int)

x = int(20)

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.13
data type(float)
x = float(20.5)

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.14
data type(complex)
x = complex(1j)

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.15
data type(list)
x = list(("apple", "banana", "cherry"))

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.16
data type(tuple)
x = tuple(("apple", "banana", "cherry"))

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.17
data type(range)
x = dict(name="John", age=36)

#display x:
print(x)

#display the data type of x:
print(type(x))

2.18
data type(dict)
x = dict(name="John", age=36)

#display x:
print(x)

#display the data type of x:
print(type(x))

2.19
data type(set)
x = set(("apple", "banana", "cherry"))

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.20
data type(frozenset)
x = frozenset(("apple", "banana", "cherry"))

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.21
data type(bool)
x = bool(5)

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.22
data type(bytes)
x = bytes(5)

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.23
data type(bytearray)
x = bytearray(5)

#display x:
print(x)

#display the data type of x:
print(type(x)) 

2.24
data type(memoryview)
x = memoryview(bytes(5))

#display x:
print(x)

#display the data type of x:
print(type(x)) 
======================================================================
3.python Number
x = 1
y = 2.8
z = 1j

print(type(x))
print(type(y))
print(type(z))

1.a
int or integer is a whole number, positive or negative, without decimals of unlimited length.
x = 1
y = 35656222554887711
z = -3255522

print(type(x))
print(type(y))
print(type(z))

1.b
Float or "floating point number" is a number, positive or negative, containing one or more
decimals.

Float can also be scientific numbers with an "e" to indicate the power of 10.

x = 35e3
y = 12E4
z = -87.7e100

print(type(x))
print(type(y))
print(type(z))

*. Complex
Complex numbers are written with a "j" as the imaginary part:
x = 3+5j
y = 5j
z = -5j

print(type(x))
print(type(y))
print(type(z))

type Conversion
can convert from one type to another with the int(), float(), and complex() methods

x = 1 #int
y = 2.8 #float
z = 1j #complex

#convert from int to float:
a = float(x)

#convert from float to int:
b = int(y)

#convert from int to complex:
c = complex(x)

print(a)
print(b)
print(c)

print(type(a))
print(type(b))
print(type(c))
=======================================================
4.python casting
specify a variable type
casting in python is therefore done using constructor functions:
-->int()- constructs an integer number from an integer literal, a float literal
(by removing all decimals), or a string literal (providing the string represents a whole number)

-->floating()- constructs a float number from an integer literal, a float lteral or a string
literal (providing the string represents a float or an integer)

--> str() - constructs a string from a wide variety of data types, including strings, integer
literals and float literals.

1.a(int)
x = int(1)
y = int(2.8)
z = int("3")
print(x)
print(y)
print(z)

2.b(float)
x = float(1)
y = float(2.8)
z = float("3")
w = float("4.2")
print(x)
print(y)
print(z)
print(w)

2.c(str)
x = str("s1")
y = str(2)
z = str(3.0)
print(x)
print(y)
print(z)
============================================================
5.python string
Strings in python are surrounded by either single quotation marks, or double quotation marks.

'hello' is the same as "hello".

You can display a string literal with the print() function:

#You can use double or single quotes:

print("Hello")
print('Hello')

1.a
assign string to a variable
assigning a string to a variable is done with the variable name followed by an equal 
sign and the string

a = "Hello"
print(a)

*. Multpline strings
you can assign a multiline string to a variable by using 3 quotes:

a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a)

or three single quotes

a = '''Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua.'''
print(a)

*. strings are Arrays
strngs in python are arrays of bytes representing unicode character

a = "Hello, World!"
print(a[1])

*.Looping through a string
strings are arrays, we can loop through the character in a string, with a for loop.
for x in "banana":
  print(x) 

string length
To get the length of a string, use the len() function.
a = "Hello, World!"
print(len(a))

*.check string
txt = "The best things in life are free!"
print("free" in txt)

*. if statement
txt = "The best things in life are free!"
if "free" in txt:
  print("Yes, 'free' is present.")

*.check if NOT
To check if a certain phrase or character is NOT present in a string, 
we can use the keyword not in.

txt = "The best things in life are free!"
print("expensive" not in txt)

*.Use it in an if statement:
txt = "The best things in life are free!"
if "expensive" not in txt:
  print("Yes, 'expensive' is NOT present.")
  ===========================================================================
  6.python-Slicing strings

*.slicing
You can return a range of characters by using the slice syntax.

Specify the start index and the end index, separated by a colon, to return a part of the string.

b = "Hello, World!"
print(b[2:5])

*.slice from the start
By leaving out the start index, the range will start at the first character:

b = "Hello, World!"
print(b[:5])

*.slice to the End
b = "Hello, World!"
print(b[2:])

*.Negative Indexing
Use negative indexes to start the slice from the end of the string:

b = "Hello, World!"
print(b[-5:-2])
============================================================
7.Modify Strings

*.Upper Case:
a = "Hello, World!"
print(a.upper())

*.lower Case
a = "Hello, World!"
print(a.lower())

*.Remove Whitespace
whitespace is the before and/or after the actual text, and very often you want to remove this space.

a = " Hello, World! "
print(a.strip()) # returns "Hello, World!"

*.Replace string
a = "Hello, World!"
print(a.replace("H", "J"))

*.Split string:
a = "Hello, World!"
print(a.split(",")) # returns ['Hello', ' World!']
=====================================================================
8.String Concatenation:
to concatenate or combine two strings you can use + operator

a = "Hello"
b = "World"
c = a + b
print(c)

* to add a space between them, add a " ":
a = "Hello"
b = "World"
c = a + " " + b
print(c)
=====================================================
9.Format - Strings
we can combine strings and numbers by using the format() method

age = 36
txt = "My name is John, and I am {}"
print(txt.format(age))

quantity = 3
itemno = 567
price = 49.95
myorder = "I want {} pieces of item {} for {} dollars."
print(myorder.format(quantity, itemno, price))

*.index numbers {0} to be sure the arguments are placed in the correct placeholders:
quantity = 3
itemno = 567
price = 49.95
myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
print(myorder.format(quantity, itemno, price))
=================================================================================

11.String Methods

11.2
string casefold() method
Syntax:string.casefold()

txt = "Hello, And Welcome To My World!"

x = txt.casefold()

print(x)
=======================================
11.3
string center() method
txt = "banana"

x = txt.center(20)

print(x)

the Center() method 
Syntax :sring.center(Length, character)

txt = "banana"

x = txt.center(20, "O")

print(x)

================================================
11.4
Sting count() method
Return the number of times the value "apple" appears in the string:
txt = "I love apples, apple are my favorite fruit"

x = txt.count("apple")

print(x)

DEF: the count() method returns the number of times a specified value
appears in the string.
syntax: string.count(value, start, end)

Parameter	Description
value	Required. A String. The string to value to search for
start	Optional. An Integer. The position to start the search. Default is 0
end	Optional. An Integer. The position to end the search. 
Default is the end of the string

txt = "I love apples, apple are my favorite fruit"

x = txt.count("apple", 10, 24)

print(x)
=============================
11.5
String encode() method:
txt = "My name is Ståle"

x = txt.encode()

print(x)

Def and usage
the encode() :using specified encoding. if no encoding is specified,
Syntax:
string:
string.encode(encoding=encoding, errors=errors)

*.parameter values

Parameter	Description
encoding	Optional. A String specifying the encoding to use. Default is UTF-8
errors	Optional. A String specifying the error method. Legal values are:
'backslashreplace'	- uses a backslash instead of the character that could not be encoded
'ignore'	- ignores the characters that cannot be encoded
'namereplace'	- replaces the character with a text explaining the character
'strict'	- Default, raises an error on failure
'replace'	- replaces the character with a questionmark
'xmlcharrefreplace'	- replaces the character with an xml character


*.txt = "My name is Ståle"

print(txt.encode(encoding="ascii",errors="backslashreplace"))
print(txt.encode(encoding="ascii",errors="ignore"))
print(txt.encode(encoding="ascii",errors="namereplace"))
print(txt.encode(encoding="ascii",errors="replace"))
print(txt.encode(encoding="ascii",errors="xmlcharrefreplace"))
========================================================
11.6
String endswith() method
txt = "Hello, welcome to my world."

x = txt.endswith(".")

print(x)

DEF
endswith() method returns true if the string ends with specified value
Syntax
string.endswith(value, start,end)

parameter values
Parameter	Description
value	Required. The value to check if the string ends with
start	Optional. An Integer specifying at which position to start the search
end	Optional. An Integer specifying at which position to end the search

ex:1
txt = "Hello, welcome to my world."

x = txt.endswith("my world.")

print(x)

ex:2
txt = "Hello, welcome to my world."

x = txt.endswith("my world.")

print(x)
=================================
11.7
Sring expandtabs() method
txt = "H\te\tl\tl\to"

x =  txt.expandtabs(2)

print(x)

DEF:
the expandtabs method sets the tab size to the specified number of whitespaces.
syntax:
string.expandtabs(tabsize)

parameter values

Parameter	Description
tabsize	Optional. A number specifying the tabsize. Default tabsize is 8

txt = "H\te\tl\tl\to"

print(txt)
print(txt.expandtabs())
print(txt.expandtabs(2))
print(txt.expandtabs(4))
print(txt.expandtabs(10))

=========================================
11.8
String find() method
txt = "Hello, welcome to my world."

x = txt.find("welcome")

print(x)

DEF:
The find() method finds the first occurrence of the specified value.

The find() method returns -1 if the value is not found.

The find() method is almost the same as the index() method, 
the only difference is that the index() method

Syntax:
string.find(value, start, end)

Parameter values:
Parameter	Description
value	Required. The value to search for
start	Optional. Where to start the search. Default is 0
end	Optional. Where to end the search. Default is to the end of the string

example:
txt = "Hello, welcome to my world."

x = txt.find("e")

print(x)

ex2:
txt = "Hello, welcome to my world."

x = txt.find("e", 5, 10)

print(x)

ex3
txt = "Hello, welcome to my world."

print(txt.find("q"))
print(txt.index("q"))
=======================================
11.9
String format() method
txt = "For only {price:.2f} dollars!"
print(txt.format(price = 49))

DEF:
The format() method formats the specified value(s) and insert them inside the string's placeholder.

The placeholder is defined using curly brackets: {}. Read more about the placeholders in the Placeholder section below.

The format() method returns the formatted string

Synatx:
string.format(value1, value2...)

parameter:
Parameter	Description
value1, value2...	Required. One or more values that should be formatted and inserted in the string. The values can be A number specifying the position of the element you want to remove.

The values are either a list of values separated by commas, a key=value list, or a combination of both.

The values can be of any data type.

#named indexes:
txt1 = "My name is {fname}, I'm {age}".format(fname = "John", age = 36)
#numbered indexes:
txt2 = "My name is {0}, I'm {1}".format("John",36)
#empty placeholders:
txt3 = "My name is {}, I'm {}".format("John",36)

print(txt1)
print(txt2)
print(txt3)

Formatting Types
Inside the placeholders you can add a formatting type to format the result:

:<		Left aligns the result (within the available space)
:>		Right aligns the result (within the available space)
:^		Center aligns the result (within the available space)
:=		Places the sign to the left most position
:+		Use a plus sign to indicate if the result is positive or negative
:-		Use a minus sign for negative values only
: 		Use a space to insert an extra space before positive numbers (and a minus sign befor negative numbers)
:,		Use a comma as a thousand separator
:_		Use a underscore as a thousand separator
:b		Binary format
:c		Converts the value into the corresponding unicode character
:d		Decimal format
:e		Scientific format, with a lower case e
:E		Scientific format, with an upper case E
:f		Fix point number format
:F		Fix point number format, in uppercase format (show inf and nan as INF and NAN)
:g		General format
:G		General format (using a upper case E for scientific notations)
:o		Octal format
:x		Hex format, lower case
:X		Hex format, upper case
:n		Number format
:%		Percentage format
=========================================================================

12.Python Booleans:
booleans represent one of two values: true or false

print(10 > 9)
print(10 == 9)
print(10 < 9)

*.
a = 200
b = 33

if b > a:
  print("b is greater than a")
else:
  print("b is not greater than a")

*.Evaluate Values and Variable
the bool() function allows you to evaluate any value,
and give you true or false in return

print(bool("Hello"))
print(bool(15))

Ex:
x = "Hello"
y = 15

print(bool(x))
print(bool(y))

ex
bool("abc")
bool(123)
bool(["apple", "cherry", "banana"])

ex3
bool(False)
bool(None)
bool(0)
bool("")
bool(())
bool([])
bool({})

ex 4
class myclass():
  def __len__(self):
    return 0

myobj = myclass()
print(bool(myobj))

*.function can return a Boolean

Ex1:
def myFunction() :
  return True

if myFunction():
  print("YES!")
else:
  print("NO!")
======================================================
13.
python Operators:

print(10 + 5)

Arithmetic operators
Assignment operators
Comparison operators
Logical operators
Identity operators
Membership operators
Bitwise operators

1.a
Sub
x = 5
y = 3

print(x - y)

1.c
Multiplication	
x = 5
y = 3

print(x * y)

1.d
Division
x = 12
y = 3

print(x / y)

1.e
Modulus
x = 5
y = 2

print(x % y)

1.f
Exponentiation	
x = 2
y = 5

print(x ** y) #same as 2*2*2*2*2

1.g

x = 15
y = 2

print(x // y)
Floor division
#the floor division // rounds the result down to the nearest whole number

*.Assignment oper

1.1
x = 5

print(x)

1.2
x = 5

x += 3

print(x)

1.3
x = 5

x -= 3

print(x)

1.4
x = 5

x *= 3

print(x)

1.5

	
x = 5

x /= 3

print(x)

1.6
x = 5

x%=3

print(x)

1.7
x = 5

x//=3

print(x)

1.8
x = 5

x **= 3

print(x)

1.9
x = 5

x &= 3

print(x)

1.10
x = 5

x |= 3

print(x)

1.11
x = 5

x ^= 3

print(x)

1.12
x = 5

x >>= 3

print(x)


1.13
x = 5

x <<= 3

print(x)

*. comparsion oper
1.a
x = 5
y = 3

print(x == y)

# returns False because 5 is not equal to 3

1.b
x = 5
y = 3

print(x != y)

# returns True because 5 is not equal to 3

1.c
x = 5
y = 3

print(x > y)

# returns True because 5 is greater than 3

1.d
x = 5
y = 3

print(x < y)

# returns False because 5 is not less than 3

1.e
x = 5
y = 3

print(x >= y)

# returns True because five is greater, or equal, to 3

1.f
x = 5
y = 3

print(x <= y)

# returns False because 5 is neither less than or equal to 3

*.python logical oper
1.a
x = 5

print(x > 3 and x < 10)

# returns True because 5 is greater than 3 AND 5 is less than 10

1.b
x = 5

print(x > 3 or x < 4)

# returns True because one of the conditions are true
 (5 is greater than 3, but 5 is not less than 4)

1.c
x = 5

print(not(x > 3 and x < 10))

# returns False because not is used to reverse the result

*. Identity oper
x = ["apple", "banana"]
y = ["apple", "banana"]
z = x

print(x is z)

# returns True because z is the same object as x

print(x is y)

# returns False because x is not the same object as y,
 even if they have the same content

print(x == y)

# to demonstrate the difference betweeen "is" and "==":
 this comparison returns True because x is equal to y

ex2
x = ["apple", "banana"]
y = ["apple", "banana"]
z = x

print(x is not z)

# returns False because z is the same object as x

print(x is not y)

# returns True because x is not the same object as y,
 even if they have the same content

print(x != y)

# to demonstrate the difference betweeen "is not" and "!=": 
this comparison returns False because x is equal to y
==============================================================
14.
Python lists:
thislist = ["apple", "banana", "cherry"]
print(thislist)

*. List Length
To determine how many items a list has, use the len() function:
thislist = ["apple", "banana", "cherry"]
print(len(thislist))

*.data types
list1 = ["apple", "banana", "cherry"]
list2 = [1, 5, 7, 9, 3]
list3 = [True, False, False]

*.type()
mylist = ["apple", "banana", "cherry"]
print(type(mylist))

*. the list() constructor
thislist = list(("apple", "banana", "cherry")) # note the double round-brackets
print(thislist)
========================================================================
15.
Access items
thislist = ["apple", "banana", "cherry"]
print(thislist[1])

*.Negative indexing
thislist = ["apple", "banana", "cherry"]
print(thislist[-1])

*.range of Indexes
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:5])
=================================================================================
16. 
change list itr

thislist = ["apple", "banana", "cherry"]
thislist[1] = "blackcurrant"
print(thislist)

ex1
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "mango"]
thislist[1:3] = ["blackcurrant", "watermelon"]
print(thislist)

ex2
thislist = ["apple", "banana", "cherry"]
thislist[1:2] = ["blackcurrant", "watermelon"]
print(thislist)

*.Insert
thislist = ["apple", "banana", "cherry"]
thislist.insert(2, "watermelon")
print(thislist)
==============================================================
17.
Add list items

*.Append Items

thislist = ["apple", "banana", "cherry"]
thislist.append("orange")
print(thislist)

*.Insert Items
thislist = ["apple", "banana", "cherry"]
thislist.insert(1, "orange")
print(thislist)

ex1
thislist = ["apple", "banana", "cherry"]
tropical = ["mango", "pineapple", "papaya"]
thislist.extend(tropical)
print(thislist)

*.add any Iterable
thislist = ["apple", "banana", "cherry"]
thistuple = ("kiwi", "orange")
thislist.extend(thistuple)
print(thislist)

=====================================================================
18.
Remove list Items:

thislist = ["apple", "banana", "cherry"]
thislist.remove("banana")
print(thislist)

*. Remove  specified Index
the pop()
thislist = ["apple", "banana", "cherry"]
thislist.pop(1)
print(thislist)

ex1
thislist = ["apple", "banana", "cherry"]
thislist.pop()
print(thislist)

Ex:
del
thislist = ["apple", "banana", "cherry"]
del thislist[0]
print(thislist)

ex1
thislist = ["apple", "banana", "cherry"]
del thislist

*
clear the list
thislist = ["apple", "banana", "cherry"]
thislist.clear()
print(thislist)
==================================================================
19.
Loop through a list
thislist = ["apple", "banan", "cherry"]
for x in thislist:
print(x)

*.Loop through the index numbers
Use the range() and len() functions to create a suitable iterable.

this
list = ["apple", "banana", "cherry"]
for i in range(len(thislist)):
  print(thislist[i])

*. using a while loop
You can loop through the list items by using a while loop.

thislist = ["apple", "banana", "cherry"]
i = 0
while i < len(thislist):
  print(thislist[i])
  i = i + 1

*Looping Using liat comprehension

thislist = ["apple", "banana", "cherry"]
[print(x) for x in thislist]
====================================================

















  







