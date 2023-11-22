---
title: Example Guide
description: A guide in my new Starlight docs site.
---

# The Complete Python Master Guide v3

# Introduction

Python is an easy to learn yet extremely powerful programming language used for web development, data science, AI, automation, and building all kinds of applications. This comprehensive guide will take you from beginner to advanced Python master.
#Python is a way to tell computers what to do. It can be used to make websites, games, and apps.

# Getting Started
# Why Learn Python?
# Python is used for:

#Web development - building websites, web apps, backends
#Data science/AI - analyzing data, machine learning
#Automation - automating tasks with scripts
#Software development - building desktop apps, games
#Python code is simple and readable, similar to everyday English. This makes Python a great first language for beginners to learn programming.

#Python is also versatile and can be used to build almost anything you can imagine. Learning Python provides a solid programming foundation and advanced capabilities for data science, AI, and more.

#Install Python
#Go to python.org and download the latest version of Python 3.
#Follow the installation wizard, checking the box to add Python to your system path.
#Open a terminal and run python --version to verify it is installed or not.

python --version

#It should print out the version of Python 3.8.10.
#That's it! Python is now ready to use on your system.

#Your First Python Program
#Let's start by writing a simple Python program:

print("Hello World!")

#This uses the print() function to output text. Save it as hello.py and run it to see "Hello World!" printed.

#Python Basics
#Now that Python is installed, let's go over the fundamental building blocks:

#Variables
#Variables store data in Python:

name = "John" # String
age = 25 # Integer 
price = 18.95 # Float

#name, age, and price are examples of variables holding different data types.

#Data Types
#Main data types in Python:

Strings - Text enclosed in quotes. "Hello"
Integers - Whole numbers like 1, 2, 3.
Floats - Decimals like 1.5, 5.67.
Booleans - True/False values.
Lists - Ordered sequence like [1, 2, 3].
Dictionaries - Unordered key-value pairs like {"name":"John"}.

x = 5               # int
y = 5.0             # float
z = "Hello"         # str
a = [1, 2, 3]       # list
b = (1, 2, 3)       # tuple
c = {"one": 1, "two": 2}  # dict

#Operators
#Operators perform actions on variables and values:

+ Addition
- Subtraction
* Multiplication
/ Division
% Modulus/remainder
== Equal to
!= Not equal
> Greater than
< Less than

Arithmetic operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`
Assignment operators: `=`, `+=`, `-=`, `*=`, `/=`, `//=`, `%=`, `**=`
Comparison operators: `==`, `!=`, `<`, `>`, `<=`, `>=`
Logical operators: `and`, `or`, `not`

x = 5       # assignment operator
y = 10
z = x + y   # arithmetic operator
if z == 15:  # comparison operator
  print("z is 15")

#This assigns x and y, adds them, and checks if z is 15.

# Membership Operators
a = [1, 2, 3]
if 1 in a:           # 'in' operator
  print("1 is in the list a")

# This checks if 1 is in the list a.

if 4 not in a:       # 'not in' operator
  print("4 is not in the list a")

# This checks if 4 is not in the list a.

# Logical Operators

x = 5
y = 10
if x > 3 and y > 3:  # 'and' operator
  print("Both x and y are greater than 3")

# This checks if both x and y are greater than 3.

if x > 3 or y > 3:   # 'or' operator
  print("At least one of x or y is greater than 3")

# This checks if either x or y is greater than 3.

if not x > 10:       # 'not' operator
  print("x is not greater than 10")

# This checks if x is not greater than 10.   

# Identity Operators
if x is y:           # 'is' operator
  print("x and y are the same")

# This checks if x and y are the same object.

if x is not y:       # 'is not' operator
  print("x and y are not the same")

#This assigns x and y, adds them, and checks if z is 15.

#Conditional Logic
#Conditional logic executes code based on whether conditions are met:

age = 20

if age >= 18:
  print("You are an adult")
else:
  print("You are a minor")

#This checks if age is 18+ and prints a message.

#Loops
#Loops repeat code multiple times:

#For Loop

for i in range(5): 
  print(i)

#This prints 0 to 4 by looping 5 times.

#While Loop

x = 0
while x < 5:
  print(x) 
  x += 1

#This loops while x is less than 5, incrementing x each time.

#Functions
#Functions are reusable blocks of code:

def say_hi(name):
  print("Hi " + name)
  
say_hi("John") # Call function

# This defines a function called say_hi that prints a message.
# say_hi accepts a name parameter and prints "Hi" + name.

#Importing
#Import statements allow you to import code from other files:

import helpers 

helpers.say_hi("John")

#This imports the say_hi function from helpers.py

#Intermediate Python
#You now know Python basics. Let's cover some more advanced topics:

#Lists
#Lists store ordered collections of data:

names = ["John", "Sarah", "Mark"]

#Access items by index starting from 0:

print(names[0]) # First item

#Common list operations:

len(list) - Get length
list.append() - Add item to end
list.insert() - Insert item at index
list.remove() - Remove item by value

#Dictionaries
#Dictionaries store unordered key-value pairs:

person = {"name":"John", "age":25}

#Access values using keys:

print(person["name"])

#Common dictionary operations:

len(dict) - Number of items
dict[key] = val - Set value for key
del dict[key] - Delete key-value pair
dict.keys() - Get list of keys

#Classes
#Classes define object templates with methods:

class Person:

  def __init__(self, name, age):
    self.name = name
    self.age = age
    
  def say_hi(self):
    print("Hi, I am", self.name)

p1 = Person("John", 36)
p1.say_hi()

# __init__ initializes each new instance
# self refers to the current instance
#Create objects by calling the class

#Handling Files
#Python can read and write files:

#Read File

file = open("data.txt", "r")
print(file.read())
file.close()

#Write File

file = open("data.txt", "w")
file.write("Hello World")
file.close()

#Specify "r" for reading or "w" for writing.

#Exceptions
#Exceptions handle errors in Python:

try:
  num = int(input("Enter a number: "))
except ValueError:
  print("Invalid number")

#This catches the ValueError for invalid input.

#You can define custom exceptions by inheriting from Exception.
#Advanced Python
#Now that you have a solid base in Python, let's go over some more advanced programming topics:

#Lambda Functions
#Lambdas are anonymous functions defined with a single line:

double = lambda x: x * 2
print(double(5)) # 10

#This creates a function that doubles a number.

#List Comprehensions
#List comprehensions provide concise syntax for creating lists:

nums = [x*2 for x in range(10)]

#This creates a list of doubled numbers from 0 to 9.

# Decorators
# Decorators modify the behavior of functions:

def decorate(func):
  def wrapper():
    print("Before calling")
    func()
    print("After calling")
  return wrapper

@decorate
def my_func():
  print("Hello World")
  
my_func()

# This decorates my_func() to add extra behavior.

# Generators
# Generators produce sequences of values over time:

def counter(max):
  num = 0
  while num < max:
    yield num
    num += 1

#Create generator objects and iterate through values:

gen = counter(10)
for x in gen:
  print(x) # Prints 0 to 9

# Virtual Environments
# Virtual environments isolate project dependencies:

python3 -m venv myenv
source myenv/bin/activate
pip install <packages>

#Activate the virtual environment before installing packages.