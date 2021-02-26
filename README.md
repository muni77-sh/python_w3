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





