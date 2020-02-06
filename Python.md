# Python
[Prepared by Konrapp Software Solutions Private Limited](http://konrapp.in "Konrapp's Website")

The course is divided into 6 interactive sessions, where the student will learn `python` by doing. The **first session** we will introduce python and get familiar with its `syntax`. In the **second session** we will learn to create custom `functions`. **Session 3** will focus on `control statements` and `boolean algerbra`. **Session 4** introduces the students to data structures and particularly `lists`. **Session 5** will focus completely on iterative and conditional `loops`. In the **final session** students will be guided to create various real life `projects` where they will apply all the knowledge acquired throughout the course. All sessions will have a `quiz` to assess student understanding periodically.

## Table of Contents

### Session 1
1. Introduction
2. Syntax
    1. Comments
    2. Print
    3. Strings
    4. Variables
    5. Errors
    6. Numbers
    7. Calculations
    8. Changing Numbers
    9. Exponents
    10. Modulo
    11. Concatenation
    12. Plus Equals
    13. Multi-line Strings
    14. Review
    15. Quiz

### Session 2
3. Introduction to Functions
    1. What is a function
    2. Write a function
    3. Whitespace
    4. Parameters
    5. Multiple Parameters
    6. Keyword Arguments
    7. Returns
    8. Multiple Return Values
    9. Scope
    10. Review
    11. Quiz

### Session 3
4. Control Flow
    1. Boolean Expressions
    2. Relational Operators I
    3. Boolean Variables
    4. If Statements
    5. Relational Operators II
    6. Boolean Operators: and
    7. Boolean Operators : or
    8. Boolean Operators : not
    9. Else Statements
    10. Else if Statements
    11. Try and Except Statements
    12. Review
    13. Quiz

### Session 4
5. Lists
    1. What is a list
    2. Lists II
    3. List of Lists
    4. Zip
    5. Emplty Lists
    6. Growing a List: Append
    7. Growing a List: Plus(+)
    8. Range I
    9. Range II
    10. Review
    11. Quiz
6. Working with Lists
    1. Operations on Lists
    2. Length of a list
    3. Selecting List Elements I
    4. Selecting List Elements II
    5. Slicing Lists
    6. Slicing Lists II
    7. Counting elements in a list
    8. Sorting Lists I
    9. Sorting Lists II
    10. Review
    11. Quiz

### Session 5
7. Loops
    1. Introduction
    2. Create a For Loop
    3. Using Range in Loops
    4. Infinite Loops
    5. Break
    6. Continue
    7. While Loops
    8. Nested Loops
    9. List Comprehensions
    10. More List Comprehensions
    11. Review
    12. Quiz

### Session 6
8. Freeform Projects
    1. Create Purchasing Information and Receipts for Lovely Loveseats
    2. Getting Ready for Physics Class
    3. Sal's Shipping
    4. Python Gradebook
    5. Len's Slice
    6. Carly's Clippers

## Introduction 
**Welcome**
Python is a programming language. Like other languages, it gives us a way to communicate ideas. In the case of a programming language, these ideas are “commands” that people use to communicate with a computer!

We convey our commands to the computer by writing them in a text file using a programming language. These files are called programs. Running a program means telling a computer to read the text file, translate it to the set of operations that it understands, and perform those actions.

In order to run python code we need a compiler, which will translate code into output. Try this [online compiler to get started.](https://repl.it/languages/python3 "Free Online Python Compiler")

**Instructions**
Change `Konrapp` to your name in the script to the right. Run the code to see what it does! As soon as you’re ready, we will move on to the next exercise to begin learning to write your own Python programs!

```python
my_name = "Konrapp"
print("Hello and welcome " + my_name + "!")
```

## Syntax
In this course we’ll learn about the syntax of the Python programming language! We will go over fundamental commands that store variables, print messages, and perform mathematical operations.

### Comments
Ironically, the first thing we’re going to do is show how to tell a computer to ignore a part of a program. Text written in a program but not run by the computer is called a comment. Python interprets anything after a `#` as a comment.

Comments can:
- Provide context for why something is written the way it is:
```python
# This variable will be used to count the number of times anyone tweets the word persnickety
persnickety_count = 0
```
- Help other people reading the code understand it faster:
```python
# This code will calculate the likelihood that it will rain tomorrow
complicated_rain_calculation_for_tomorrow()
```
- Ignore a line of code and see how a program will run without it:
```python
# useful_value = old_sloppy_code()
useful_value = new_clean_code()
```
### Print
Now what we’re going to do is teach our computer to communicate. The gift of speech is valuable: a computer can answer many questions we have about “how” or “why” or “what” it is doing. In Python, the `print()` function is used to tell a computer to talk. The message to be printed should be surrounded by quotes:

```python
# from Mary Shelley's Frankenstein
print("There is something at work in my soul, which I do not understand.")
```
In the above example, we direct our program to `print()` an excerpt from a notable book. The printed words that appear as a result of the `print()` function are referred to as *output*. The output of this example program would be:

```
There is something at work in my soul, which I do not understand.
```
**Instructions**
Print the distinguished greeting “Hello world!”

### Strings
Computer programmers refer to blocks of text as *strings*. In our last exercise, we created the string “Hello world!”. In Python a string is either surrounded by double quotes (`"Hello world"`) or single quotes (`'Hello world'`). It doesn’t matter which kind you use, just be consistent.

**Instructions**
1 Print your name using the print() command.
2 If your print statement uses double-quotes `"`, change them to single-quotes `'`. If it uses single-quotes `'`, change them to double-quotes `"`.

Try running your code again after switching the type of quote-marks. Is anything different about the output?

Typically, either single or double quotes can be used interchangeably for creating a string. However, in certain situations, the type of quotes can matter, depending on the content of the string itself. If the string contains single quotes, it can be more convenient to wrap the entire string in double quotes. And if the string contains double quotes, you might use single quotes to wrap the string instead.

The reason for this is that each string starts and ends when a pair of quotes is encountered. If there is another matching quote within the string, that may end the string prematurely, causing errors.

```python
# Examples of valid strings
print("I'm coding!")
print('The computer printed the string "Hello!"')

# Example of invalid string 
print("A common phrase in programming is "Hello world"")
```

### Variables
Programming languages offer a method of storing data for reuse. If there is a greeting we want to present, a date we need to reuse, or a user ID we need to remember we can create a *variable* which can store a value. In Python, we *assign* variables by using the equals sign (`=`).

```python
message_string = "Hello there"
# Prints "Hello there"
print(message_string)
```

In the above example, we store the message “Hello there” in a variable called `message_string`. Variables can’t have spaces or symbols in their names other than an underscore (`_`). They can’t begin with numbers but they can have numbers after the first letter (e.g., `cool_variable_5` is OK).

It’s no coincidence we call these creatures “variables”. If the context of a program changes, we can update a variable but perform the same logical process on it.

```python
# Greeting
message_string = "Hello there"
print(message_string)

# Farewell
message_string = "Hasta la vista"
print(message_string)
```

Above, we create the variable `message_string`, assign a welcome message, and print the greeting. After we greet the user, we want to wish them goodbye. We then update `message_string` to a departure message and print that out.

**Instructions**
Update the variable `meal` to reflect each meal of the day before we print it.

```python
# We've defined the variable "meal" here to the name of the food we ate for breakfast!
meal = "Dosa"

# Printing out breakfast
print("Breakfast:")
print(meal)

# Now update meal to be lunch!
meal = 

# Printing out lunch
print("Lunch:")
print(meal)

# Now update "meal" to be dinner

# Printing out dinner
print("Dinner:")
print(meal)
```

### Errors
Humans are prone to making mistakes. Humans are also typically in charge of creating computer programs. To compensate, programming languages attempt to understand and explain mistakes made in their programs.

Python refers to these mistakes as errors and will point to the location where an error occurred with a `^` character. When programs throw errors that we didn’t expect to encounter we call those errors `bugs`. Programmers call the process of updating the program so that it no longer produces unexpected errors `debugging`.

Two common errors that we encounter while writing Python are `SyntaxError` and `NameError`.

- `SyntaxError` means there is something wrong with the way your program is written — punctuation that does not belong, a command where it is not expected, or a missing parenthesis can all trigger a `SyntaxError`.
- A `NameError` occurs when the Python interpreter sees a word it does not recognize. Code that contains something that looks like a variable but was never defined will throw a `NameError`.

**Instructions**
You might encounter a `SyntaxError` if you open a string with double quotes and end it with a single quote. Update the string so that it starts and ends with the same punctuation.
```python
print('This message has mismatched quote marks!")
```
You might encounter a `NameError` if you try to print a single word string but fail to put any quotes around it. Python expects the word of your string to be defined elsewhere but can’t find where it’s defined. Add quotes to either side of the string to squash this bug.
```python
print(Abracadabra)
```
Update the malformed strings in the workspace to all be strings.

### Numbers
Computers can understand much more than just strings of text. Python has a few numeric *data types*. It has multiple ways of storing numbers. Which one you use depends on your intended purpose for the number you are saving.

An *integer*, or `int`, is a whole number. It has no decimal point and contains all counting numbers (1, 2, 3, …) as well as their negative counterparts and the number 0. If you were counting the number of people in a room, the number of jellybeans in a jar, or the number of keys on a keyboard you would likely use an integer.

A *floating-point number*, or a `float`, is a decimal number. It can be used to represent fractional quantities as well as precise measurements. If you were measuring the length of your bedroom wall, calculating the average test score of a seventh-grade class, or storing a cricket player’s batting average for the 1998 season you would likely use a `float`.

Numbers can be assigned to variables or used literally in a program:

```python
an_int = 2
a_float = 2.1

print(an_int + 3)
# prints 5
```
Above we defined an integer and a float as the variables `an_int` and `a_float`. We printed out the sum of the variable `an_int` with the number 3. We call the number 3 here a *literal*, meaning it’s actually the number `3` and not a variable with the number 3 assigned to it.

Floating-point numbers can behave in some unexpected ways due to how computers store them. For more information on floating-point numbers and Python, review [Python’s documentation on floating-point limitations.](https://docs.python.org/3/tutorial/floatingpoint.html "Python 3 Documentation")

**Instructions**
A recent movie-going experience has you excited to publish a review. You rush out of the cinema and hastily begin programming to create your movie-review website: *The Big Screen’s Greatest Scenes Decided By A Machine*.

1 Create the following variables and assign integer numbers to them: `release_year` and `runtime`.
2 Now, create the variable `rating_out_of_10` and assign it a float number between one and ten.

### Calculations
Computers absolutely excel at performing calculations. The “compute” in their name comes from their historical association with providing answers to mathematical questions. Python performs addition, subtraction, multiplication, and division with `+`, `-`, `*`, and `/`.

```python
# Prints "500"
print(573 - 74 + 1)

# Prints "50"
print(25 * 2)

# Prints "2.0"
print(10 / 5)
```

Notice that when we perform division, the result has a decimal place. This is because Python converts all `int`s to `float`s before performing division. In older versions of Python (2.7 and earlier) this conversion did not happen, and integer division would always round down to the nearest integer.

Division can throw its own special error: `ZeroDivisionError`. Python will raise this error when attempting to divide by 0.

Mathematical operations in Python follow the standard mathematical [order of operations.](https://en.wikipedia.org/wiki/Order_of_operations.html 'Wikipedia Bodmas Article')

**Instructions**
Print out the result of this equation: `25 * 68 + 13 / 28`

### Changing Numbers
Variables that are assigned numeric values can be treated the same as the numbers themselves. Two variables can be added together, divided by `2`, and multiplied by a third variable without Python distinguishing between the variables and *literals* (like the number `2` in this example). Performing arithmetic on variables does not change the variable — you can only update a variable using the `=` sign.

```python
coffee_price = 1.50
number_of_coffees = 4

# Prints "6.0"
print(coffee_price * number_of_coffees)
# Prints "1.5"
print(coffee_price)
# Prints "4"
print(number_of_coffees)

# Updating the price 
coffee_price = 2.00

# Prints "8.0"
print(coffee_price * number_of_coffees)
# Prints "2.0"
print(coffee_price)
# Prints "4"
print(number_of_coffees)
```
We create two variables and assign numeric values to them. Then we perform a calculation on them. This doesn’t update the variables! When we update the `coffee_price` variable and perform the calculations again, they use the updated values for the variable!

**Instructions**
1 You’ve decided to get into quilting! To calculate the number of squares you’ll need for your first quilt let’s create two variables: `quilt_width` and `quilt_length`. Let’s make this first quilt 8 squares wide and 12 squares long.
2 Print out the number of squares you’ll need to create the quilt!
3 It turns out that quilt required a little more material than you have on hand! Let’s only make the quilt 8 squares long. How many squares will you need for this quilt instead?

### Exponents
Python can also perform exponentiation. In written math, you might see an exponent as a superscript number, but typing superscript numbers isn’t always easy on modern keyboards. Since this operation is so related to multiplication, we use the notation `**`.

```python
# 2 to the 10th power, or 1024
print(2 ** 10)

# 8 squared, or 64
print(8 ** 2)

# 9 * 9 * 9, 9 cubed, or 729
print(9 ** 3)

# We can even perform fractional exponents
# 4 to the half power, or 2
print(4 ** 0.5)
```
Here, we compute some simple exponents. We calculate 2 to the 10th power, 8 to the 2nd power, 9 to the 3rd power, and 4 to the 0.5th power.

**Instructions**
You really like how the square quilts from last exercise came out, and decide that all quilts that you make will be square from now on.

1 Using the exponent operator, print out how many squares you’ll need for a 6x6 quilt, a 7x7 quilt, and an 8x8 quilt.
2 Your 6x6 quilts have taken off so well, 6 people have each requested 6 quilts. Print out how many tiles you would need to make 6 quilts apiece for 6 people.

### Modulo
Python offers a companion to the division operator called the modulo operator. The modulo operator is indicated by `%` and gives the remainder of a division calculation. If the number is divisible, then the result of the modulo operator will be 0.

```python
# Prints 4 because 29 / 5 is 5 with a remainder of 4
print(29 % 5)

# Prints 2 because 32 / 3 is 10 with a remainder of 2
print(32 % 3)

# Modulo by 2 returns 0 for even numbers and 1 for odd numbers
# Prints 0
print(44 % 2)
```
Here, we use the modulo operator to find the remainder of division operations. We see that `29 % 5` equals 4, `32 % 3` equals 2, and `44 % 2` equals 0.

The modulo operator is useful in programming when we want to perform an action every nth-time the code is run. Can the result of a modulo operation be larger than the divisor? Why or why not?

**Instructions**
1 You’re trying to divide a group into four teams. All of you count off, and you get number 27.

Find out your team by computing 27 modulo 4. Save the value to `my_team`.

2 Print out `my_team`. What number team are you on?

3 Food for thought: what number team are the two people next to you (26 and 28) on? What are the numbers for all 4 teams?

### Concatenation
The `+` operator doesn’t just add two numbers, it can also “add” two strings! The process of combining two strings is called *string concatenation*. Performing string concatenation creates a brand new string comprised of the first string’s contents followed by the second string’s contents (without any added space in-between).

```python
greeting_text = "Hey there!"
question_text = "How are you doing?"
full_text = greeting_text + question_text

# Prints "Hey there!How are you doing?"
print(full_text)
```
In this sample of code, we create two variables that hold strings and then concatenate them. But we notice that the result was missing a space between the two, let’s add the space in-between using the same concatenation operator!

```python
full_text = greeting_text + " " + question_text

# Prints "Hey there! How are you doing?"
print(full_text)
```
Now the code prints the message we expected.

If you want to concatenate a string with a number you will need to make the number a string first, using the `str()` function. If you’re trying to `print()` a numeric variable you can use commas to pass it as a different argument rather than converting it to a string.

```python
birthday_string = "I am "
age = 10
birthday_string_2 = " years old today!"

# Concatenating an integer with strings is possible if we turn the integer into a string first
full_birthday_string = birthday_string + str(age) + birthday_string_2

# Prints "I am 10 years old today!"
print(full_birthday_string)

# If we just want to print an integer 
# we can pass a variable as an argument to 
# print() regardless of whether 
# it is a string.

# This also prints "I am 10 years old today!"
print(birthday_string, age, birthday_string_2)
```

Using `str()` we can convert variables that are not strings to strings and then concatenate them. But we don’t need to convert a number to a string for it to be an argument to a print statement.

**Instructions**
Concatenate the strings and save the message they form in the variable `message`.

```python
string1 = "The wind, "
string2 = "which had hitherto carried us along with amazing rapidity, "
string3 = "sank at sunset to a light breeze; "
string4 = "the soft air just ruffled the water and "
string5 = "caused a pleasant motion among the trees as we approached the shore, "
string6 = "from which it wafted the most delightful scent of flowers and hay."
```
Now print the `message` to see the result

### Plus Equals

Python offers a shorthand for updating variables. When you have a number saved in a variable and want to add to the current value of the variable, you can use the `+=` (plus-equals) operator.

```python
# First we have a variable with a number saved
number_of_miles_hiked = 12

# Then we need to update that variable
# Let's say we hike another two miles today
number_of_miles_hiked += 2

# The new value is the old value
# Plus the number after the plus-equals
print(number_of_miles_hiked)
# Prints 14
```

Above, we keep a running count of the number of miles a person has gone hiking over time. Instead of recalculating from the start, we keep a grand total and update it when we’ve gone hiking further.

The plus-equals operator also can be used for string concatenation, like so:

```python
hike_caption = "What an amazing time to walk through nature!"

# Almost forgot the hashtags!
hike_caption += " #nofilter"
hike_caption += " #blessed"
```

We create the social media caption for the photograph of nature we took on our hike, but then update the caption to include important social media tags we almost forgot.

**Instructions**
We’re doing a little bit of online shopping and find a pair of new sneakers. Right before we check out, we spot a nice sweater and some fun books we also want to purchase!

Use the `+=` operator to update the `total_price` to include the prices of `nice_sweater` and `fun_books`.

```python
total_price = 0

new_sneakers = 50.00

total_price += new_sneakers

nice_sweater = 39.00
fun_books = 20.00
# Update total_price here:

print("The total price is", total_price)
```

### Multi-line Strings
Python strings are very flexible, but if we try to create a string that occupies multiple lines we find ourselves face-to-face with a `SyntaxError`. Python offers a solution: multi-line strings. By using three quote-marks (`"""` or `'''`) instead of one, we tell the program that the string doesn’t end until the next triple-quote. This method is useful if the string being defined contains a lot of quotation marks and we want to be sure we don’t close it prematurely.

```python
leaves_of_grass = """
Poets to come! orators, singers, musicians to come!
Not to-day is to justify me and answer what I am for,
But you, a new brood, native, athletic, continental, greater than
  before known,
Arouse! for you must justify me.
"""
```

In the above example, we assign a famous poet’s words to a variable. Even though the quote contains multiple linebreaks, the code works!

If a multi-line string isn’t assigned a variable or used in an expression it is treated as a comment.

**Instructions**

Assign the string 
```
Stranger, if you passing meet me and desire to speak to me, why
  should you not speak to me?
And why should I not speak to you?
```
to the variable `to_you` and print the output.

### Review

In this section, we accomplished a lot of things! We instructed our computers to print messages, we stored these messages as variables, and we learned to update those messages depending on the part of the program we were in. We performed mathematical calculations and explored some of the mathematical expressions that Python offers us. We learned about errors and other valuable skills that will continue to serve us as we develop our programming skills.

Good job!

**Instructions**
Create variables:

* `my_age`
* `half_my_age`
* `greeting`
* `name`
* `greeting_with_name`

Assign values to each using your knowledge of division and concatenation!

### Quiz
What is the value of `total_cost` that gets printed?

```python
total_cost = 5
total_cost += 10
print(total_cost)
```

Which of the following defined variables is a string?

```python
cool_variable_1 = 23.18
cool_variable_2 = 9
cool_variable_3 = "Important Message!"
cool_variable_4 = 14 ** 3
```

What is Python syntax for creating a variable and assigning the number `10` to it?
How does one define a multi-line string in Python?
What is the value of `modulo_variable` in the following expression?

```python
modulo_variable = 14 % 4
```

Which function outputs text to the terminal?
What is the output of the following code?
```python
cool_number = 12 + 30
cool_number * 5
print(cool_number)
```

How do you combine two strings?
What character begins a comment in Python?
What is the difference between a float and an int?
What happens when running the following code?
```python
message = What a cool message!
print(message)
```

What number is saved to exponented_variable in the following expression?
```python
exponented_variable = 2 ** 4
```

## Functions
### Introduction to Functions

A *function* is a collection of several lines of code. By *calling* a function, we can call all of these lines of code at once, without having to repeat ourselves.

So, a function is a tool that you can use over and over again to produce consistent output from different inputs.

We have already learned about one function, called `print`. We know that we call `print` by using this syntax:

```python
print(something_to_print)
```

In the rest of the lesson, we’ll learn how to build more functions, call them with and without inputs, and return values from them.

### What is a Function?

Let’s imagine that we are creating a program that greets customers as they enter a grocery store. We want a big screen at the entrance of the store to say:

```
Welcome to Engrossing Grocers.
Our special is mandarin oranges.
Have fun shopping!
```

We have learned to use print statements for this purpose:

```python
print("Welcome to Engrossing Grocers.")
print("Our special is mandarin oranges.")
print("Have fun shopping!")
```

Every time a customer enters, we call these three lines of code. Even if only 3 or 4 customers come in, that’s a lot of lines of code required.

In Python, we can make this process easier by assigning these lines of code to a *function*. We’ll name this function `greet_customer`. In order to call a function, we use the syntax `function_name()`. The parentheses are important! They make the code inside the function run. In this example, the function call looks like:

```python
greet_customer()
```

Every time we call `greet_customer()`, we would see:

```
Welcome to Engrossing Grocer's.
Our special is mandarin oranges.
Have fun shopping!
```

Having this functionality inside `greet_customer()` is better form, because we have isolated this behavior from the rest of our code. Once we determine that `greet_customer()` works the way we want, we can reuse it anywhere and be confident that it greets, without having to look at the implementation. We can get the same output, with less repeated code. Repeated code is generally more error prone and harder to understand, so it’s a good goal to reduce the amount of it.

**Instructions**

We have made a function for you called `sing_song`. Call this function once to see what it prints out.

```python
def sing_song():
  print("You may say I'm a dreamer")
  print("But I'm not the only one")
  print("I hope some day you'll join us")
  print("And the world will be as one")
```

Now call `sing_song` a second time.

### Write a Function

We have seen the value of simple functions for modularizing code. Now we need to understand how to write a function. To write a function, you must have a heading and an indented block of code. The heading starts with the keyword `def` and the name of the function, followed by parentheses, and a colon. The indented block of code performs some sort of operation. This syntax looks like:

```python
def function_name():
  some code
```

For our `greet_customer()` example, the function definition looks like:

```python
def greet_customer():
  print("Welcome to Engrossing Grocers.")
  print("Our special is mandarin oranges.")
  print("Have fun shopping!")

greet_customer()
# prints greeting lines
```

The keyword `def` tells Python that we are defining a function. This function is called `greet_customer`. Everything that is indented after the `:` is what is run when `greet_customer()` is called. So every time we call `greet_customer()`, the three `print` statements run.

**Instructions**

Write a function called `loading_screen` that prints `"This page is loading..."` to the console.
Outside of the function body (unindented), call `loading_screen()`.

### Whitespace

Consider this function:

```python```
def greet_customer():
    print("Welcome to Engrossing Grocers.")
    print("Our special is mandarin oranges.")
    print("Have fun shopping!")
```

The three `print` statements are all executed together when `greet_customer()` is called. This is because they have the same level of indentation. In Python, the amount of whitespace tells the computer what is part of a function and what is not part of that function. If we wanted to write another line outside of `greet_customer()`, we would have to unindent the new line:

```python
def greet_customer():
    print("Welcome to Engrossing Grocers.")
    print("Our special is mandarin oranges.")
    print("Have fun shopping!")
print("Cleanup on Aisle 6")
```

When we call `greet_customer`, the message`"Cleanup on Aisle 6"` is not printed, as it is not part of the function.

**Instructions**
Run the script below. Look at what is printed out!

```python
def about_this_computer():
  print("This computer is running on version Everest Puma")
  print("This is your desktop")

about_this_computer()
```

Remove the indent on the second print statement. Run the file. Now what’s printed?

### Parameters

Let’s return to Engrossing Grocers. The special of the day will not always be mandarin oranges, it will change every day. What if we wanted to call these three print statements again, except with a variable special? We can use *parameters*, which are variables that you can pass into the function when you call it.

```python
def greet_customer(special_item):
    print("Welcome to Engrossing Grocers.")
    print("Our special is " + special_item + ".")
    print("Have fun shopping!")
```

In the definition heading for `greet_customer()`, the `special_item` is referred to as a *formal parameter*. This variable name is a placeholder for the name of the item that is the grocery’s special today. Now, when we call `greet_customer`, we have to provide a `special_item`:

```python
greet_customer("peanut butter")
```
That item will get printed out in the second print statement:

```
Welcome to Engrossing Grocers.
Our special is peanut butter.
Have fun shopping!
```

The value between the parentheses when we call the function (in this case, `"peanut butter"`) is referred to as an argument of the function call. The argument is the information that is to be used in the execution of the function. When we then call the function, Python assigns the formal parameter name `special_item` with the actual parameter data, `"peanut_butter"`. In other words, it is as if this line was included at the top of the function:

```python
special_item = "peanut butter"
```

Every time we call `greet_customer()` with a different value between the parentheses, `special_item` is assigned to hold that value.

**Instructions**
The function `mult_two_add_three()` prints a number multiplied by `2` and added to `3`. As it is written right now, the `number` that it operates on is always `5`.

```python
def mult_two_add_three():
  number = 5
  print(number*2 + 3)
```

1. Call the function and see what it prints to the console.
2. Now, modify the function definition so that it has a parameter called `number`. Then delete the `number = 5` assignment on the first line of the function.

Pass the number `1` into your function call.
3. Call the function with the value `5` as the argument.
4. Call the function with the value `-1` as the argument.
5. Call the function with the value `0` as the argument.

### Multiple Paramenters

Our grocery greeting system has gotten popular, and now other supermarkets want to use it. As such, we want to be able to modify both the special item and the name of the grocery store in a greeting like this:

```
Welcome to [grocery store].
Our special is [special item].
Have fun shopping!
```
We can make a function take more than one parameter by using commas:

```python
def greet_customer(grocery_store, special_item):
    print("Welcome to "+ grocery_store + ".")
    print("Our special is " + special_item + ".")
    print("Have fun shopping!")
```
The variables `grocery_store` and `special_item` must now both be provided to the function upon calling it:

```python
greet_customer("Stu's Staples", "papayas")
```
which will print:

```
Welcome to Stu's Staples.
Our special is papayas.
Have fun shopping!
```
**Instructions**

The function `mult_two_add_three` takes a number, multiplies it by two and adds three. We want to make this more flexible. 

```python
def mult_two_add_three(number):
  print(number*2 + 3)
```  

1. First, change the name of the function to `mult_x_add_y`.
2. Now, add `x` and `y` as parameters of the function, after `number`.
3. Inside the function, replace `2` in the print statement with `x`, and replace `3` in the print statement with `y`.
4. Call the function with these values:

`number: 5`

`x: 2`

`y: 3`
5. Call the function with these values:

`number: 1`

`x: 3`

`y: 1`

### Keyword Arguements

In our `greet_customer()` function from the last exercise, we had two arguments:

```python
def greet_customer(grocery_store, special_item):
    print("Welcome to "+ grocery_store + ".")
    print("Our special is " + special_item + ".")
    print("Have fun shopping!")
```
Whichever value is put into `greet_customer()` first is assigned to `grocery_store`, and whichever value is put in second is assigned to `special_item`. These are called *positional arguments* because their assignments depend on their positions in the function call.

We can also pass these arguments as *keyword arguments*, where we explicitly refer to what each argument is assigned to in the function call.

```python
greet_customer(special_item="chips and salsa", grocery_store="Stu's Staples")
```
```
Welcome to Stu's Staples.
Our special is chips and salsa.
Have fun shopping!
```

We can use keyword arguments to make it explicit what each of our arguments to a function should refer to in the body of the function itself.

We can also define default arguments for a function using syntax very similar to our keyword-argument syntax, but used during the function definition. If the function is called without an argument for that parameter, it relies on the default.

```python
def greet_customer(special_item, grocery_store="Engrossing Grocers"):
    print("Welcome to "+ grocery_store + ".")
    print("Our special is " + special_item + ".")
    print("Have fun shopping!")
```

In this case, `grocery_store` has a default value of `"Engrossing Grocers"`. If we call the function with only one argument, the value of `"Engrossing Grocers"` is used for `grocery_store`:

```python
greet_customer("bananas")
```
```
Welcome to Engrossing Grocers.
Our special is bananas.
Have fun shopping!
```

Once you give an argument a default value (making it a keyword argument), no arguments that follow can be used positionally. For example:

```python
def greet_customer(special_item="bananas", grocery_store): # this is not valid
    ...

def greet_customer(special_item, grocery_store="Engrossing Grocers"): # this is valid
    ...
```

**Instructions**

We have defined a function `create_spreadsheet`, which just takes in a `title`, and prints that it is creating a spreadsheet.

```python
# Define create_spreadsheet():
def create_spreadsheet(title):
  print("Creating a spreadsheet called "+title)

# Call create_spreadsheet() below with the required arguments:
create_spreadsheet("Downloads")
```

1. Run the code to see the function work on an input of `"Downloads"`.
2. Add the parameter `row_count` to the function definition. Set the default value to be `1000`.
3. Change the print statement in the function to print “Creating a spreadsheet called `title` with `row_count` rows”, where title and row_count are replaced with their respective values.
4. Call `create_spreadsheet()` with title set to `"Applications"` and row_count set to `10`.

### Returns

So far, we have only seen functions that print out some result to the console. Functions can also return a value to the user so that this value can be modified or used later. When there is a result from a function that can be stored in a variable, it is called a *returned* function value. We use the keyword `return` to do this.

Here’s an example of a function `divide_by_four` that takes an integer argument, divides it by four, and `return`s the result:

```python
def divide_by_four(input_number):
    return input_number/4
```

The program that calls `divide_by_four` can then use the result later:

```python
result = divide_by_four(16)
# result now holds 4
print("16 divided by 4 is " + str(result) + "!")
result2 = divide_by_four(result)
print(str(result) + " divided by 4 is " + str(result2) + "!")
```
This would print out:

```
16 divided by 4 is 4!
4 divided by 4 is 1!
```
In this example, we returned a number, but we could also return a String:

```python
def create_special_string(special_item):
    return "Our special is " + special_item + "."

special_string = create_special_string("banana yogurt")

print(special_string)
```

```
Our special is banana yogurt.
```

**Instructions**
The function `calculate_age` below creates a variable called `age` that is the difference between the current year, and a birth year, both of which are inputs of the function.

1. Add a line to return `age`.
2. Outside of the function, call `calculate_age` with values `2049` (`current_year`) and `1993` (`birth_year`) and save the value to a variable called `my_age`.
3. Call `calculate_age` with values `2049` (`current_year`) and `1953` (`birth_year`) and save the value to a variable called `dads_age`.
4. Print the string `"I am X years old and my dad is Y years old"` to the console, with `my_age` where the `X` is and `dads_age` where the `Y` is.

### Multiple Return Values

Sometimes we may want to return more than one value from a function. We can return several values by separating them with a comma:

```python
def square_point(x_value, y_value):
  x_2 = x_value * x_value
  y_2 = y_value * y_value
  return x_2, y_2
```

This function takes in an x value and a y value, and returns them both, squared. We can get those values by assigning them both to variables when we call the function:

```python
x_squared, y_squared = square_point(1, 3)
print(x_squared)
print(y_squared)
```
This will print:

```
1
9
```

**Instructions**
1. Write a function called `get_boundaries()` that takes in two parameters, a number called `target` and a number called `margin`.

It should create two variables:

`low_limit`: `target` minus the `margin`
`high_limit`: `margin` added to `target`
2. Return both `low_limit` and `high_limit` from the function, in that order.
3. Call the function on the target `100` with a margin of `20`. Save the returned values to variables called `low` and `high`.

### Scope

Let’s say we have our function from the last exercise that creates a string about a special item:

```python
def create_special_string(special_item):
    return "Our special is " + special_item + "."
```

What if we wanted to access the variable `special_item` outside of the function? Could we use it?

```python
def create_special_string(special_item):
    return "Our special is " + special_item + "."

print("I don't like " + special_item)
```

If we try to run this code, we will get a NameError, telling us that `'special_item' is not defined`. The variable `special_item` has only been defined inside the space of a function, so it does not exist outside the function. We call the part of a program where `special_item` can be accessed its scope. The scope of `special_item` is only the `create_special_string` function.

Variables defined outside the scope of a function may be accessible inside the body of the function:

```python
header_string = "Our special is " 

def create_special_string(special_item):
    return header_string + special_item + "."
print(create_special_string("grapes"))
```
There is no error here. `header_string` can be used inside the `create_special_string` function because the scope of `header_string` is the whole file. This file would produce:
```
Our special is grapes.
```

**Instructions**
Outside of the function `calculate_age()`, try to print `current_year`. 
```python
def calculate_age(current_year, birth_year):
  age = current_year - birth_year
  return age
  ```

1. Does it work?
2. What about `age`? Outside of `calculate_age()`, try to print `age`. Does it work?
3. No! Even though we return `age` at the end of the function, the variable `age` still only exists within the context of the function.
Remove both print statements
4. Let’s try something different. Remove the parameter `current_year` so that it is no longer a parameter of `calculate_age()`.
5. It’s the year 2048.

Define `current_year` as a variable BEFORE defining the function and give it the value `2048`. Now, every time `calculate_age()` is called, it should only take `birth_year`.
6. Try to print `current_year` one last time. Does it work finally?
7. Hooray! Now we have `current_year` globally defined. Great work!

Let’s make sure our function still works: print the value of `calculate_age()` with `1970` as the argument.

### Review

Great! So far you have learned:

How to write a function
How to give a function inputs
How to return values from a function
What scope means
Let’s practice these concepts again so that you won’t forget them!

**Instructions**

1. Define a function called `repeat_stuff` that takes in two inputs, stuff, and `num_repeats`.

We will want to make this function print a string with `stuff` repeated `num_repeats` amount of times. For now, only put an empty `print` statement inside the function.
2. Outside of the function, call `repeat_stuff`.

You can use the value `"Row "` for `stuff` and `3` for `num_repeats`.
3. Change the `print` statement inside `repeat_stuff` to a `return` statement instead.

It should return `stuff*num_repeats`.

**Note:** Multiplying a string just makes a new string with the old one repeated! For example:
```python
"na"*6
```
results in the string `"nananananana"`.
4. Give the parameter `num_repeats` a default value of `10`.
5. Add `repeat_stuff("Row ", 3)` and the string "Your Boat. " together and save the result to a variable called `lyrics`.
6. Create a variable called `song` and assign it the value of `repeat_stuff` called with the singular input `lyrics`.
7. Print `song`.

1. Given the following function, what will produce the output `"There is no greater agony than bearing an untold story inside you."`?

```python
def quote(x):
  print("There is no greater agony than bearing " + x + " inside you.")
```

2. What line of code can be used to return a variable `inner_var` from a function back to the piece of code that called the function?
3. What line of code will call `force` with a value of `10` for `mass` and a value of `9.81` for `acceleration`? 
```python
def force(mass, acceleration):
  force_val = mass*acceleration
  return force_val
```
4. How do you call a function called `setup` with no arguments?
5. What happens when you call `report`?
```python
time = "3pm"
mood = "good"

def report():
  print("The current time is " + time)
  print("The mood is " + mood)

print("End of report")
```
6. How do you call `update` with a `new_value` of `20`?
```python
def update(new_value = 10):
  old_value = new_value
```
7. Which variables can be called in the blank spot in this code:
```python
counter = 0

def update():
  new_counter = counter + 1
  return new_counter

_______
```





## Control Flow

### Introduction

Imagine waking up in the morning.

You wake up and think,

“Ugh, is it a weekday?”

If so, you have to get up and get dressed and get ready for work or school. If not, you can sleep in a bit longer and catch a couple extra Z’s. But alas, it is a weekday, so you are up and dressed and you go to look outside, “What’s the weather like? Do I need an umbrella?”

These questions and decisions control the flow of your morning, each step and result is a product of the conditions of the day and your surroundings. Your computer, just like you, goes through a similar flow every time it executes code. A program will run (wake up) and start moving through its checklists, is this condition met, is that condition met, okay let’s execute this code and return that value.

This is the *Control Flow* of your program. In Python, your script will execute from the top down, until there is nothing left to run. It is your job to include gateways, known as conditional statements, to tell the computer when it should execute certain blocks of code. If these conditions are met, then run this function.

Over the course of this lesson, you will learn how to build conditional statements using boolean expressions, and manage the control flow in your code.

### Boolean Expressions

In order to build control flow into our program, we want to be able to check if something is true or not. A boolean expression is a statement that can either be `True` or `False`.

Let’s go back to the ‘waking up’ example. The first question, “Is today a weekday?” can be written as a boolean expression:

```
Today is a weekday.
```
This expression can be `True` if today is Tuesday, or it can be `False` if today is Saturday. There are no other options.

Consider the phrase:

```
Friday is the best day of the week.
```
Is this a boolean expression?

No, this statement is an opinion and is not objectively `True` or `False`. Someone else might say that “Wednesday is the best weekday,” and their statement would be no less `True` or `False` than the one above.

How about the phrase:

```
Sunday starts with the letter 'C'.
```

Is this a boolean expression?

Yes! This expression can only be `True` or `False`, which makes it a boolean expression. Even though the statement itself is false (Sunday starts with the letter ‘C’), it is still a boolean expression.

**Instructions**

Determine if the following statements are boolean expressions or not. If they are, set the matching variable to the right to `"Yes"` and if not set the variable to `"No"`. Here’s an example of what to do:

Example statement:
```
My dog is the cutest dog in the world.
```
This is an opinion and not a boolean expression, so you would set `example_statement` to `"No"` in the editor to the right. Okay, now it’s your turn:

Statement one:
```
Dogs are mammals.
```
Statement two:
```
My dog is named Pavel.
```
Statement three:
```
Dogs make the best pets.
```
Statement four:
```
Cats are female dogs.
```

```python
example_statement = "No"

statement_one =

statement_two =  

statement_three = 

statement_four = 
```

### Relational Operators: Equals and Not Equals

Now that we understand what boolean expressions are, let’s learn to create them in Python. We can create a boolean expression by using *relational operators*.

Relational operators compare two items and return either `True` or `False`. For this reason, you will sometimes hear them called *comparators*.

The two boolean operators we’ll cover first are:

Equals: `==`
Not equals: `!=`
These operators compare two items and return `True` or `False` if they are equal or not.

We can create boolean expressions by comparing two values using these operators:
```python
>>> 1 == 1
True
>>> 2 != 4
True
>>> 3 == 5
False
>>> '7' == 7
False
```
Each of these is an example of a boolean expression. `>>>` is the prompt when you run Python in your terminal, which you can then use to evaluate simple expressions, such as these.

Why is the last statement false? The `''` marks in `'7'` make it a string, which is different from the integer value `7`, so they are not equal. When using relational operators it is important to always be mindful of type.

**Instructions**

Determine if the following boolean expressions are `True` or `False`. Input your answer as `True` or `False` in the appropriate variable to the right.

Statement one:

```python
(5 * 2) - 1 == 8 + 1
```
Statement two:
```python
13 - 6 != (3 * 2) + 1
```
Statement three:
```python
3 * (2 - 1) == 4 - 1
```

### Boolean Variables

Before we go any further, let’s talk a little bit about `True` and `False`. You may notice that when you type them in the code editor (with uppercase T and F), they appear in a different color than variables or strings. This is because `True` and `False` are their own special type: `bool`.

`True`` and `False` are the only `bool` types, and any variable that is assigned one of these values is called a *boolean variable*. Boolean variables can be created in several ways. The easiest way is to simply assign `True` or `False` to a variable:
```python
set_to_true = True
set_to_false = False
```
You can also set a variable equal to a boolean expression.
```python
bool_one = 5 != 7 
bool_two = 1 + 1 != 2
bool_three = 3 * 3 == 9
```
These variables now contain boolean values, so when you reference them they will only return the `True` or `False` values of the expression they were assigned.
```python
>>>bool_three
True
>>>bool_four
False
>>>bool_five
True
```

**Instructions**
1. Create a variable named `my_baby_bool` and set it equal to "true".
2. Check the type of my_baby_bool using `type(my_baby_bool)`.

You’ll have to print it to get the results to display in the terminal.

### If Statements

“Okay okay okay, boolean variables, boolean expressions, blah blah *blah*, I thought I was learning how to build control flow into my code!”

You are, I promise you!

Understanding boolean variables and expressions is essential because they are the building blocks of *conditional statements*.

Recall the waking-up example from the beginning of this lesson. The decision-making process of “Is it raining? If so, bring an umbrella” is a conditional statement. Here it is phrased in a different way:

```
If it is raining then bring an umbrella.
```
Can you pick out the boolean expression here?

Right, `"it is raining"` is the boolean expression, and this conditional statement is checking to see if it is True.

If `"it is raining" == True` then the rest of the conditional statement will be executed and you will bring an umbrella.

This is the form of a conditional statement:
```
If [it is raining] then [bring an umbrella]
```

In Python, it looks very similar:
```python
if is_raining:
  bring_umbrella()
```

You’ll notice that instead of “then” we have a colon, `:`. That tells the computer that what’s coming next is what should be executed if the condition is met. Let’s take a look at another conditional statement:

```python
if 2 == 4 - 2: 
  print("apple")
```

Will this code print `apple` to the terminal? Yes, because the condition of the `if` statement, `2 == 4 - 2` is `True`.

Let’s work through a couple more together:

1. Below there is a function with an `if` statement. I wrote this function because my coworker Dave kept using my computer without permission and he is a real doofus. It takes `user_name` as an input and if the user is Dave it tells him to stay off my computer.

Enter a user name in the field for `user_name` and try running the function.

2. Oh no! We got a `SyntaxError`! This happens when we make a small error in the syntax of the conditional statement.

Read through the error message carefully and see if you can find the error. Then, fix it, and run the code again.

3. Ugh! Dave got around my security and has been logging onto my computer using our coworker Angela’s user name, `angela_catlady_87`.

Update the function with a second `if` statement so it checks for this user name as well and returns

```python
 "I know it is you Dave! Go away!"
 ```
in response. That’ll teach him!



## Lists

Learn about lists, a data structure in Python used to store ordered groups of data.

```python
primes = [2, 3, 5, 7, 11]
print(primes)

empty_list = []
```
In Python, lists are ordered collections of items that allow for easy use of a set of data.

List values are placed in between square brackets `[ ]`, separated by commas. It is good practice to put a space in between the comma and the next value. The values in a list do not need to be unique (the same value can be repeated).

Empty lists do not contain any values within the square brackets.

### Creating and Modifying a list in Python

#### What is a list?

A *list* is an ordered set of objects in Python.

Suppose we want to make a list of the heights of students in a class:

- Jenny is 61 inches tall
- Alexus is 70 inches tall
- Sam is 67 inches tall
- Grace is 64 inches tall

In Python, we can create a variable called `heights` to store these numbers

```python
heights = [61, 70, 67, 64]
```

Notice that:

1. A list begins and ends with square brackets (`[` and `]`).
2. Each item (i.e., `67` or `70`) is separated by a comma (`,`)
3. It’s considered good practice to insert a space (``) after each comma, but your code will run just fine if you forget the space.

**Instructions**
```python
heights = [61, 70, 67, 64]

# broken_heights = [65 71 59 62]
```
1.A new student just joined the class:

- Cole is 65 inches tall

Add Cole’s height to the end of the list `heights`.

2. Remove the `#` in front of the definition of the list `broken_heights`. If you run this code, you’ll get an error:

```python
SyntaxError: invalid syntax
```
Add commas (`,`) to `broken_heights` so that it runs without errors.

#### Lists II

Lists can contain more than just numbers.

Let’s revisit our height example:

- Jenny is 61 inches tall
- Alexus is 70 inches tall
- Sam is 67 inches tall
- Grace is 64 inches tall

We can make a list of strings that contain the students’ names:
```python
names = ['Jenny', 'Alexus', 'Sam', 'Grace']
```
We can also combine multiple data types in one list. For example, this list contains both a string and an integer:
```python
mixed_list = ['Jenny', 61]
```

**Instructions**
```python
ints_and_strings = [1, 2, 3, 'four', 'five']
```
1. Add any string to the list `ints_and_strings`.
2. Create a new list called sam_height that contains:    
 - The string `'Sam'`
 - The number `67`

#### List of Lists

We’ve seen that the items in a list can be numbers or strings. They can also be other lists!

Once more, let’s return to our class height example:

- Jenny is 61 inches tall
- Alexus is 70 inches tall
- Sam is 67 inches tall
- Grace is 64 inches tall

Previously, we saw that we could create a list representing both Jenny’s name and height:

```python
jenny = ['Jenny', 61]
```
We can put several of these lists into one list, such that each entry in the list represents a student and their height:
```python
heights = [['Jenny', 61], ['Alexus', 70], ['Sam', 67], ['Grace', 64]]
```

**Instructions**
```python
heights = [['Jenny', 61], ['Alexus', 70], ['Sam', 67], ['Grace', 64]]
```
1. A new student named `'Vik'` has joined our class. Vik is `68` inches tall. Add a sublist to `heights` that represents Vik and his height.
2. Create a list of lists called `ages` where each sublist contains a student’s name and their age. Use the following data:

- `'Aaron'` is `15`
- `'Dhruti'` is `16`

#### Zip

Again, let’s return to our class height example:

- Jenny is 61 inches tall
- Alexus is 70 inches tall
- Sam is 67 inches tall
- Grace is 64 inches tall

Suppose that we already had a list of names and a list of heights:

```python
names = ['Jenny', 'Alexus', 'Sam', 'Grace']
heights = [61, 70, 67, 65]
```

If we wanted to create a list of lists that paired each name with a height, we could use the command `zip`. `zip` takes two (or more) lists as inputs and returns an *object* that contains a list of pairs. Each *pair* contains one element from each of the inputs. You won’t be able to see much about this object from just printing it:

```python
names_and_heights = zip(names, heights)
print(names_and_heights)
```
because it will return the location of this object in memory. Output would look something like this:

```python
<zip object at 0x7f1631e86b48>
```

To see the nested lists, you can convert the zip object to a `list` first:

```python
print(list(names_and_heights))
```
returns:

```python
[('Jenny', 61), ('Alexus', 70), ('Sam', 67), ('Grace', 65)]
```



## Classes
### Types

Python equips us with many different ways to store data. A `float` is a different kind of number from an `int`, and we store different data in a `list` than we do in a `dict`. These are known as different *types*. We can check the type of a Python variable using the `type()` function.

```python
a_string = "Cool String"
an_int = 12

print(type(a_string))
# prints "<class 'str'>"

print(type(an_int))
# prints "<class 'int'>"
```

Above, we defined two variables, and checked the `type` of these two variables. A variable’s type determines what you can do with it and how you can use it. You can’t `.get()` something from an integer, just as you can’t add two dictionaries together using `+`. This is because those operations are defined at the `type` level.

**Instructions**
- Call `type()` on the integer `5` and print the results.
- Define a dictionary `my_dict`.
- Print out the `type()` of `my_dict`.
- Define a list called `my_list`.
- Print out the `type()` of `my_list`.

### Class

A *class* is a template for a data type. It describes the kinds of information that class will hold and how a programmer will interact with that data. Define a class using the `class` keyword. PEP 8 Style Guide for Python Code recommends capitalizing the names of classes to make them easier to identify.

```python
class CoolClass:
  pass
```

In the above example we created a class and named it `CoolClass`. We used the `pass` keyword in Python to indicate that the body of the class was intentionally left blank so we don’t cause an `IndentationError`. We’ll learn about all the things we can put in the body of a class in the next few exercises.

**Instructions**
Define an empty class called `Facade`. We’ll chip away at it soon!

### Instantiation
A class doesn’t accomplish anything simply by being defined. A class must be *instantiated*. In other words, we must create an *instance* of the class, in order to breathe life into the schematic.


Instantiating a class looks a lot like calling a function. We would be able to create an instance of our defined `CoolClass` as follows:

```python
cool_instance = CoolClass()
```

Above, we created an object by adding parentheses to the name of the class. We then assigned that new instance to the variable `cool_instance` for safe-keeping.

**Instructions**
Below we see our `Facade` class from last exercise. Make a `Facade` instance and save it to the variable `facade_1`.

```python
class Facade:
  pass
```

### Object-Oriented Programming

A class instance is also called an *object*. The pattern of defining classes and creating objects to represent the responsibilities of a program is known as *Object Oriented Programming or OOP*.

Instantiation takes a class and turns it into an object, the `type()` function does the opposite of that. When called with an object, it returns the class that the object is an instance of.

```python
print(type(cool_instance))
# prints "<class '__main__.CoolClass'>"
```

We then print out the type() of `cool_instance` and it shows us that this object is of type `__main__.CoolClass`.

In Python `__main__` means “this current file that we’re running” and so one could read the output from `type()` to mean “the class `CoolClass` that was defined here, in the script you’re currently running.”

**Instructions**
- Below we see `facade_1` from last exercise. Try calling `type()` on facade_1 and saving it to the variable `facade_1_type`.

```python
class Facade:
  pass

facade_1 = Facade()
```
- Print out `facade_1_type`.

### Class Variables
When we want the same data to be available to every instance of a class we use a *class variable*. A class variable is a variable that’s the same for every instance of the class.

You can define a class variable by including it in the indented part of your class definition, and you can access all of an object’s class variables with `object.variable` syntax.

```python
class Musician:
  title = "Rockstar"

drummer = Musician()
print(drummer.title)
# prints "Rockstar"
```

Above we defined the class `Musician`, then instantiated `drummer` to be an object of type `Musician`. We then printed out the drummer’s `.title` attribute, which is a class variable that we defined as the string “Rockstar”.

If we defined another musician, like `guitarist = Musician()` they would have the same `.title` attribute.

**Instructions**
You are digitizing grades for *Sri Gowthami Public School*. At *SGPS*, as the students call it, `65` is the minimum passing grade.

Create a `Grade` class with a class attribute `minimum_passing` equal to `65`.

### Methods

*Methods* are functions that are defined as part of a class. The first argument in a method is always the object that is calling the method. Convention recommends that we name this first argument `self`. Methods always have at least this one argument.

We define methods similarly to functions, except that they are indented to be part of the class.

```python
class Dog():
  dog_time_dilation = 7

  def time_explanation(self):
    print("Dogs experience {} years for every 1 human year.".format(self.dog_time_dilation))

pipi_pitbull = Dog()
pipi_pitbull.time_explanation()
# Prints "Dogs experience 7 years for every 1 human year."
```

Above we created a `Dog` class with a `time_explanation` method that takes one argument, `self`, which refers to the object calling the function. We created a `Dog` named `pipi_pitbull` and called the `.time_explanation()` method on our new object for Pipi.

Notice we didn’t pass any arguments when we called `.time_explanation()`, but were able to refer to self in the function body. When you call a method it automatically passes the object calling the method as the first argument.

**Instructions**
- At *SGPS*, the students are constantly calling the school rules into question. Create a `Rules` class so that we can explain the rules.
- Give `Rules` a method `washing_brushes` that returns the string .
```
"Point bristles towards the basin while washing your brushes."
```

### Methods and Arguments
Methods can also take more arguments than just `self`:

```python
class DistanceConverter:
  kms_in_a_mile = 1.609
  def how_many_kms(self, miles):
    return miles * self.kms_in_a_mile

converter = DistanceConverter()
kms_in_5_miles = converter.how_many_kms(5)
print(kms_in_5_miles)
# prints "8.045"
```
Above we defined a `DistanceConverter` class, instantiated it, and used it to convert 5 miles into kilometers. Notice again that even though `how_many_kms` takes two arguments in its definition, we only pass `miles`, because `self` is implicitly passed (and refers to the object `converter`).

***Instructions***

1. It’s March 14th (known in some places as **Pi day**) at *SGPS*, and you’re feeling awfully festive. You decide to create a program that calculates the area of a circle.

Create a `Circle` class with class variable `pi`. Set `pi` to the approximation `3.14`.

2. Give `Circle` an `area` method that takes two parameters: `self` and `radius`.

Return the area as given by this formula:

```python
area = pi * radius ** 2
```
3. Create an instance of `Circle`. Save it into the variable `circle`.
4. You go to measure several circles you happen to find around.

   - A medium pizza that is 12 inches across.
   - Your teaching table which is 36 inches across.
   - The Round Room auditorium, which is 11,460 inches across.
You save the areas of these three things into `pizza_area`, `teaching_table_area`, and `round_room_area`.

Remember that the `radius` of a circle is half the diameter. We gave three diameters here, so halve them before you calculate the given circle’s area.

### Constructors
There are several methods that we can define in a Python class that have special behavior. These methods are sometimes called “magic”, because they behave differently from regular methods. Another popular term is *dunder methods*, so-named because they have two underscores (double-underscore abbreviated to “dunder”) on either side of them.

The first dunder method we’re going to use is the `__init__` method (note the two underscores before and after the word “init”). This method is used to *initialize* a newly created object. It is called every time the class is instantiated.

Methods that are used to prepare an object being instantiated are called *constructors*. The word “constructor” is used to describe similar features in other object-oriented programming languages but programmers who refer to a constructor in Python are usually talking about the `__init__` method.















