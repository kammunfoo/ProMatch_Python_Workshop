# Teaching_Python

What do you think?

### Variables
```python
#!/usr/bin/env python3
# ^You can ignore the previous line if you are using https://repl.it/
# ^It is required for UNIX-like machines ... ignore it :)

# Adding the pound/hashtag (#) sign at the start of a line will
# make that line get ignored by the interpreter. These are called
# comments. They are essential for explaining how your code works 
# to your coworkers and also yourself (you will forget why you did things)

# a variable is a container for a value. 
# it also labels it with a descriptive name

# these are all variables
favorite_food = "Pizza"
no_slices = 8
myName = "Ashley"
myAge = 12

# the print command can be used to print variables
print(favorite_food)
print(no_slices)
print(myName)
print(myAge)

# print can also be used to print text
# the text must be within single or double quotes
print("this text is in between double quotes")
print('this text is in between single quotes')
print("""this text is in triple quotes!""")

# variable names can have a number, letters, and underscore
why_was_6_afraid_of_7 = "because 7 8 (ate) 9!"
print(why_was_6_afraid_of_7)

# all of these will cause an error. 
# variables cannot start with a number
# 789 = "this is not allowed"

# names are case sensitive
# THESE_ARE_NOT_THE_SAME != these_are_not_the_same

# variable names cannot be keywords
# for = IS NOT ALLOWED
# if = IS NOT ALLOWED
```

### Mathematical Operations
```python
# you can add numbers inside the print function
print(2 + 3)

# the asterisk sign is for multiplication
# let's calulate the area of a rectangle!
length = 10
width = 5
area = length * width
print(area)

# I have forgotten Pi ... how can I get an estimate?
# Divide 22 by 7! Division is done with /
print(22/7)

# bob has ten apples and jeff takes three
# how many apples does bob have? subtraction is done with -
bob_apples = 10
apples_stolen_by_jeff = 3
bob_apples - apples_stolen_by_jeff
print(bob_apples)

# if you pursue programming further, you'll realize
# that 2 gets raised to different powers a lot in
# binary. 2^2 = 2* 2 = 4, 2^3 = 2 * 2 * 2 = 8
# you can raise numbers to a power with **
two_raised_to_three = 2**3
print(two_raised_to_three) 
```

### Concatenating Strings
```python
# concatenation is a fancy way of saying connecting
# we want to concatenate "Python is" and " fun"
# (the space before "fun" will soon become obvious)

# this print statement will not have the correct spacing
print("Python is" + "fun")

# you need to add a space. It can be before or after the 
# first concatenating word.
print("Python is " + "fun")
print("Python is" + " fun")
```
### Basic Data Types
```python
# a string is text enclosed in quotes
this_is_a_string = "this is a string"
# an integer is a number without decimal points
this_is_an_integer = 8
# a float has decimal points
this_is_a_float = 3.14159
# a boolean is a True or False value
this_is_a_boolean = True

# you can use the python type argument to
# get the type of a variable. Here I am printing
# each type
string_type = type(this_is_a_string)
print(string_type)

integer_type = type(this_is_an_integer)
print(integer_type)

float_type = type(this_is_a_float)
print(float_type)

boolean_type = type(this_is_a_boolean)
print(boolean_type)

# you can convert types into different types
# this is converted a string "8" to an int 8
looks_like_a_number = "8"
print(looks_like_a_number)
print(type(looks_like_a_number))
looks_like_a_number = int(looks_like_a_number)
print(looks_like_a_number)
print(type(looks_like_a_number))

# this is converting a number 8 to a string "8"
print(looks_like_a_number)
print(type(looks_like_a_number))
looks_like_a_number = str(looks_like_a_number)
print(looks_like_a_number)
print(type(looks_like_a_number))

# WE SHOULD ADD CONVERTING BETWEEN BOOLEAN/STRING
# AND FLOAT/INTEGER

```

### Conditional Statements
```python
# a conditional statement checks conditions and
# then makes decisions. the Python if syntax is used for this
# keep in mind that tab-indentation is required in Python
weather_is_nice = True
if(weather_is_nice):
	print("we will go outside :)")

we_are_tired = True
if(we_are_tired):
	print("we will go to sleep")

alarm_clock_is_ringing = True
if(alarm_clock_is_ringing):
	print("turn off alarm clock")
```

### User Input
```python
# you can request user input with the input argument
name = input("What is your name? ")

print("Hello " + name + "! Welcome to Python!")

# here's a preview of equality comparisons
# they will be in the next section
if name == "David Halvorsen":
	print("you wrote this code!")

age = int(input("How old are you? "))
if age >= 18:
	print("You can vote! ")
```

### Inequality
```python
correct_password = "password"

entered_password = input("What is the password? ")

if correct_password != entered_password:
	print("incorrect password")
if correct_password == entered_password:
	print("correct password")
```

### Else Block
```python
myName = input("Enter your name: ")
if myName == "David":
	print("Yo Dave, you wrote this!")
else:
	print("Hello stranger! ... well actually, hello " + myName)
```

### Booleans
```python
sale = True
if sale:
	print("time to buy!")
else:
	print("Wait for sale")
```

### Elif
```python
stoplight = "yellow"

if stoplight == 'red':
	print("STOP")
elif stoplight == "yellow":
	print("slow down")
elif stoplight == "green":
	print("Go!")
else:
	print("I don't know what's going on!")
```

### Greet User Function
```python
def greetUser():
	myName = input("Enter username : ")

	if myName == "Alice":
		print("Hello Alice !! ")
	else:
		print("Hello " + myName)
		print("Welcome to Python programming !! ")
	storedPassword = "qwert"
	password = input("Enter your password : ")
	if password != storedPassword :
		print("Incorrect Password. Please try again.")
	else: 
		print("Welcome Alice!")
	return
greetUser()
```

### Repeating Function Calls
```python
def greetUser(myName):
	if myName == "Alice":
		print("Hello Alice")
	else:
		print("Hello " + myName)
	print("Welcome to Python programming !! ")
greetUser("Alice")
greetUser("John")
greetUser("Mary")
```

### Area Calculation Function
```python
def calcArea(length, width):
	return (length * width)
area1 = calcArea(10, 5)
area2 = calcArea(7, 3)
print(area1 - area2)
```
