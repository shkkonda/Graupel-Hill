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











