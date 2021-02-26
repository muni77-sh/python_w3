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

