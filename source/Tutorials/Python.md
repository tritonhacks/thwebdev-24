---
layout: default
title: Python
nav_order: 3
permalink: Tutorials/Python
parent: Tutorials
has_toc: false
---

# Python Introduction
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## What is Python?

Python is a popular high-level programming language that is used in various fields such as web development, data science, and software engineering. Python is known for its readability, simplicity, and versatility.

## Print Statements

In python and like many programming languages, they have print statements. These are what you can use to make the program display an output to the computer screen when you are programming.

Here's an example of a print statement that displays the words "Hello World": 

```
print("Hello World")
```
When you run the program this is the output: 
```
Hello World
```

--- 

### Comments
{: .no_toc }

In python there are these things called comments. Comments are like notes or reminders that we write in our code to help us understand it better. 

For example in python we can use a comment like this: 
```
# This is a comment
```

Here is another example of a comment being used.
```
# This code prints the words "Hello World"
print("Hello World")
```
Output:
```
Hello World
```
As we can see comments dont effect the code in any way and they are just there for you as the programmer to see. 


## Variables and Data Types

Variables in Python are like containers that hold information. Imagine a box with a label on it. You can put different things in the box, and the label helps you remember what's inside. Similarly, a variable has a name (like the label) and can store different types of information, such as numbers, words, or true/false values.

For example, let's say we have a variable called 'age' to store someone's age:

```
age = 15
```

Here, 'age' is the variable name, and '15' is the value stored in the variable. Later, if the person's age changes, we can update the variable:

```
age = 16
```

Now, 'age' holds the value '16'. Variables allow us to store and manipulate data in our programs, making them flexible and powerful."

We can also use print statements to display the information that is stored in variables. Now lets see an example.

Here we have a variable called "message" that stores the text "Hi how are you?", and a print statement with the variable "message" inside of it. 

```
message = "Hi how are you?"
print(message)
```

When we run the program this is what gets outputted:

```
Hi how are you?
```

---

In python data types are essentially different kinds of containers that store different types of information. Just like in real life, where we have different types of containers for storing different things (like a box for toys, a jar for cookies, and a bottle for water), Python has different data types for storing different kinds of information.

You can use these data types for storing different types of data in variables. 

Here are some common data types in python:

**String** (str): Strings are used for storing text, like 'hello' or 'Python is fun!'.

**Integer** (int): This data type is for storing whole numbers, like 5, 10, or -3.

**Float** (float): Floats are used for storing decimal numbers, like 3.14 or -0.5.

**Boolean** (bool): Booleans can only have two values: True or False. They're often used for making decisions in our programs, like 'Is it raining? (True/False)'.

**List**: Lists are used for storing collections of items. For example, a list of numbers [1, 2, 3] or a list of names ['Alice', 'Bob', 'Charlie'].


Here are some examples of these different data types. 

This is a variable named "message" that contains a String (str) data type.
```
message = "Hello World"
```
This is a variable named number that contains an Integer (int) data type.
```
number = 10
```
This is a variable named "decimal_number" that contains a FLoat (float) data type.
```
decimal_number = 15.5
```
This is a variable named "currently_learning" that contains a Boolean (bool) data type.
```
currently_learning = True
```
This is a list variable named "number_list" that is a list data type that contains a list of Integers. Lists can also contain Strings. 
```
number_list = [1, 2, 3]
```
---
In python we can also store a variable inside of a variable and give them new values. 

Here we have the variable age that holds the value of 15. We also have the variable called new_age that holds the value of 16.

```
age = 15
new_age = 16

print(age) 
age = new_age
print(age)
```
When the first print statement gets ran, the number 15 gets printed but when the second print statement runs, the number 16 gets printed. This is because when we did ```age = new_age```, we are giving the age variable a new value which is the value of new age. 

Output: 
```
15
16
```


## Operators

### Mathematical Operators

In Python there are arithmetic operators that are used to perform basic mathematical operations like addition, subtraction, multiplication, and division.

| Operator | Description | Syntax                                      |
| ---      | ---   | ---                                               |
| +        | Addition: adds two operands | x + y                       |
| ---      | ---   | ---                                               |
| -        | Subtraction: subtracts two operands | x - y               |
| ---      | ---   | ---                                               |
| *        | Multiplication: multiplies two operands | x * y           |
| ---      | ---   | ---                                               |
|  /       | Division: divides the first operand by the second | x / y |
| ---      | ---   | ---                                               |

Here are some examples of how to use these operators: 

```
print(5 + 5) 
print(5 - 1) 
print(5 * 5)
print(10 / 2) 
```
When we run the program all of these print statements get called and the answers to these mathematical operations get printed (outputted).

```
10 
4
25
5.0
```

We can also use variables that hold values to perform these mathematical operations.

```
number_five = 5
number_two = 2
number_one = 1
number_ten = 10

print(number_five + number_five)
print(number_five - number_one)
print(number_five * number_five)
print(number_ten / number_two)
```
Here is the output:

```
10
4
25
5.0
```
--- 

Aditionally we can use expressions which are like sentences in math that help us do calculations and solve problems. Here are some examples.

```
x = 20
y = 10
  
add = x + y 
subtract = x - y 
multiply = x * y 
divide = x / y 
  
print(add) 
print(sub) 
print(pro) 
print(div)
```

Here is what the output of this code would look like: 

```
30
10
200
2
```

--- 

In Python we can also add Strings together. This is called concatenation. Concatenation in Python is like combining pieces of text or data together to create a single, larger piece. It's like putting together pieces of a puzzle to make a bigger picture, or joining words to form a sentence.

Here is an example: 

```
word_1 = "Hello"
word_2 = "World"
print(word1 + " " + word2)
```
Output: 
```
Hello World
```

Concatenation is not limited to strings. We can also concatenate things like lists. For example:
```
list1 = [1, 2, 3]
list2 = [4, 5, 6]
combined_list = list1 + list2
print(combined_list)  
```
Output:
```
[1, 2, 3, 4, 5, 6] 
```


### Comparison Operators

In Python Comparison operators compare values. It either returns True or False according to the condition.

| Operator | Description | Syntax                                                                              |
| ---      | ---   | ---                                                                                       |
| >        | Greater than: True if the left operand is greater than the right | x > y                          |
| ---      | ---   | ---                                                                                       |
| <        | Less than: True if the left operand is less than the right | x < y                                |
| ---      | ---   | ---                                                                                       |
| ==       | Equal to: True if both operands are equal | x == y                                                |
| ---      | ---   | ---                                                                                       |
| !=       | Not equal to: True if operands are not equal | x != y                                             |
| ---      | ---   | ---                                                                                       |
| >=       | Greater than or equal to: True if the left operand is greater than or equal to the right | x >= y |
| ---      | ---   | ---                                                                                       |
| <=       | Less than or equal to: True if the left operand is less than or equal to the right | x <= y       |
| ---      | ---   | ---                                                                                       |

Here are some examples of them being used:
```
a = 15
b = 5
  
print(a > b) # since a is greater than b, the print statement returns True

print(a < b) # since a is less than b, the print statement returns False

print(a == b) # since a is not equal to b, the print statement returns False

print(a != b) # since a is not equal to b, the print statement returns True

print(a >= b) # since a is either greater than or equal to b, the print statement returns True

print(a <= b) # since a is either not less than or equal to b, the print statement returns False
```

Here is the output of this code:
```
True
False
False
True
True
False

```
### Logical Opersators

Logical operators in Python are like tools we use to make decisions in our programs. Just like how you might use the words 'and', 'or', and 'not' to combine ideas or conditions when you're making a decision in real life, logical operators in Python help us combine conditions and make decisions in our code.

| Operator | Description | Syntax                                          |
| ---      | ---   | ---                                                   |
| and      | Logical AND: True if both the operands are true | x and  y    |
| ---      | ---   | ---                                                   |
| or       | Logical OR: True if either of the operands is true  | x or y  |
| ---      | ---   | ---                                                   |
| not      | Logical NOT: True if the operand is false | not x             |
| ---      | ---   | ---                                                   |

Here are some examples on how to use them. 
```
a = True
b = False
print(a and b) # returns False because b is False. If they were both True then it would return True.

print(a or b) # returns True because at least one of them is True which in this case is a.

print(not a) # returns False because a is True. 

print(not b) # returns True because b is False. 

```

Output:
```
False 
True
False
True
```

### Identity And Membership Operators

Identity operators in Python are like tools we use to check if two things are the same or different. Just like how you might compare two things in real life to see if they are identical or not.

| Operator | Description | Syntax                                |
| ---      | ---   | ---                                         |
| is       | True if the operands are identical     | x is y     |
| ---      | ---   | ---                                         |
| is not   | True if the operands are not identical | x is not y |
| ---      | ---   | ---                                         |

Here are some examples for how we can use them.

```
a = 10
b = 20
  
print(a is b) # returns False because this is checking if a and b are the same but they are not.

print(a is not b) # returns True because this is checking if a is not equal to b which is True.
```
Output: 
```
False 
True
```
---
Membership operators in Python are like tools we use to check if something is part of a group or sequence. It's like looking for a specific item in a collection, such as finding a book in a library or checking if your name is on a list.

| Operator | Description | Syntax                                |
| ---      | ---   | ---                                         |
| in       | True if value is found in the sequence     | x in y     |
| ---      | ---   | ---                                         |
| not in   | True if value is not found in the sequence | x not in y |
| ---      | ---   | ---                                         |

Here are some examples: 

In this example we have a list of numbers and we are printing True if 6 is in the list and False if it is not. 
```
numbers = [1, 2, 3, 4, 5] 
print(6 in numbers) 
```
Output:
```
False 
```
Since 6 was not in the list, this statement prints False.

In this next example we have a list of numbers and we are printing True if 9 is not in the list and True if it is. 
```
numbers = [1, 2, 3, 4, 5] 
print(9 not in numbers) 
```
Output:
```
True
```
Since 9 was not in the list, this statement prints True.

Aditionally we can also use this for Strings. 

```
sentence = "hello how are you"
print("how" in sentence) 
```
Output:
```
True
```
This prints True because the text "<mark>how</mark>" is found inside of the text "hello <mark>how</mark> are you".

## if and else Statements

If statements in Python are like decision-making tools that help our programs make choices based on certain conditions. It is used to decide whether certain code will be executed or not.

Here is an example of the format of using an if statement. 
```
if condition:
   # code to execute if the condition is true
```

Here is an example of an if statement with code to check if a number is positive. 
```
number = 5
if number > 0: 
   print("The number " + str(number) + " is positive) 
```

Output: 
```
The number 5 is positive
```
What happend was that since the number 5 was greater than zero, it printed "The number 5 is positive" and if it wasnt then nothing would be printed since the condition would be false in that situation. We also used type conversion ```str(number)``` because we cannot add an integer and a string together so we had to convert the integer of 5 into a string so there wouldn't be an error. 

### Else Statements 
{: .no_toc }

In Python 

## Lists

## Loops 

## Functions

[Previous: HTML, CS, Javascript](HTML_CSS_JS){: .float-left .v-align-text-top}
[Next: Tutorials](../../Tutorials){: .float-right .v-align-text-top}