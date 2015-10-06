# Python for Everybody Specialization

<img src="https://d1qb2nb5cznatu.cloudfront.net/startups/i/430131-86c4ecea8ec200688933e639f890bf6d-medium_jpg.jpg?buster=1433271718" width="25" height="25">  Learn to Program and Analyze Data with Python. Develop programs to gather, clean, analyze, and visualize data.

**Courses include:**

1. **[Programming for Everybody Getting Started with Python](#1-programming-for-everybody-getting-started-with-python)**
  * [Chapter 1: Why We Program](#chapter-1-why-we-program)
  * [Chapter 2: Variables, Expressions, and Statements](#chapter-2-variables-expressions-and-statements)
  * [Chapter 3: Conditional Execution](#chapter-3-conditional-execution)
  * [Chapter 4: Functions](#chapter-4-functions)
  * [Chapter 5: Loops and Iteration](#chapter-5-loops-and-iteration)
2. **Python Data Structures**
3. **Using Python to Access Web Data**
4. **Using Databases with Python**

# 1. Programming for Everybody: Getting Started with Python

## Chapter 1: Why We Program

### Sequential Steps:
* An ordered series.

```python
x = 2
print "x is:", x

x = x+ 10
print "now x is:", x
```

### Conditional Steps:
* Carried out only under certain conditions.

```python
x = 5

if x < 10:
    print 'x is small-ish'

if x > 20:
    print 'x is large-ish'
```

### Repeated Steps:
* Iteration variables (e.g. n) that change each time through a loop.
* Often these iteration variables go through a sequence of numbers.

```python
n = 5

while n > 0:
    print 'Loop executed, n is: ', n
    n = n - 1
```

## Chapter 2: Variables, Expressions, and Statements

### Constants:
* Fixed values that don't change (e.g. numbers, letters, strings).
* Numeric constants are as you expect.
* String constants use single-quotes `'` or double-quotes `"`
* Examples: `+, 5, "dog"`

### Variables:
* Named place in memory where a programmer can store data and later retrieve the data using the variable `name`
* Programmers get to choose the names of the variables.
* You can change the contents of a variable in a later statement.
* Examples: `x = 4, y = 38.1`

#### Naming Rules:
* Must start with a letter or underscore `_`
* Must consist of letters and numbers and underscores
* Case sensitive
* Good examples: `spam`, `eggs`, `spam23`, `_speed`
* Bad examples: ~~`23spam`, `#sign`, `var.12`~~

### Mnemonic
Mnemonic standards for memory, and it is a pattern of letters, ideas, or associations that assists in remembering something. **_Best graphic ever_**:
<img width="957" alt="screen shot 2015-10-03 at 9 28 30 pm" src="https://cloud.githubusercontent.com/assets/5023024/10266155/d01caa02-6a15-11e5-99e0-785f049b4e62.png">

#### Reserved Words:
```
and
del
for
is
raise
assert
elif
from
lambda
return
break
else
global
not
try
class
except
if
or
while
continue
exec
import
pass
yield
def
finally
in
print
```
### User Input:
Instruct Python to pause and read data from a user using `raw_input`, which returns a string. For example:
```python
username = raw_input('What is your username?')
print 'Hola', username
```
Which returns:
* What is your username? `geospatialem`
* Hola geospatialem

#### Converting User Input
*Background:* In Europe they start on floor 0, higher floors go to 1, 2, 3 and lower to -1, -2, etc. In the United States they start on floor 0 and go up to 1, 2, 3 and have a basement (no negative numbers).

*Solution:* To convert the European floor to an American we can ask users to input their floor number and add one to the number. To do the conversion we must convert the user input (string) to an integer and add 1 to it. However, if the user inputs anything other than an integer the program will blow up.

```python
europeanFloor = raw_input('What European floor are you on?')
americanFloor = int(europeanFloor) + 1
print "In the United States you would be on floor number", americanFloor
```

### Comments
* To comment in Python use the `#` symbol.
* Comment on what is happening in a sequence of code.
* Commenting also helps for (perhaps temporarily) turning off a line of code

For example:
```python
# This is a Python comment
```

### Chapter Quiz
*Problem:* Write a program to prompt the user for hours and rate per hour using `raw_input` to compute gross pay. Use 35 hours and a rate of 2.75 per hour to test the program (the pay should be 96.25). You should use `raw_input` to read a string and `float()` to convert the string to a number. Do not worry about error checking or bad user data.

*Solution:*
```python
# Ask the user to input their hours and pay per hour
hoursWorked = raw_input("Enter the number of hours worked:")
payRate = raw_input("Enter your hourly pay rate:")

# Convert the user input to floats from strings
totalPay = float(hoursWorked) * float(payRate)

# Display the total pay
print totalPay
```
## Chapter 3: Conditional Execution
Executions that may, or may not be executed while running, dependent on specific statements.

### Conditional Operations
Conditional operations, or boolean expressions ask a question looking for a true/false statement. For example: Is the value '10'? The answer to the question is *true/yes* or *false/no*.

### Comparison Operators
Operators look at variables but *do not change* the variables. Operators are a means to create conditional statements.

| Python    | Meaning    |
| :------------- | :------------- |
| `<`       | Less than       |
| `<=`       | Less than or equal       |
| `==`       | Equal to      |
| `>=`      | Greater than or equal to      |
| `>`      | Greater than       |
| `!=`      | Not equal       |

### Formatting
Indentation is important in Python! Some text editors turn tabs into space, make sure this feature is enabled in your text editor! **_Python depends on indents and you can get syntax errors even when everything looks fine due to indentation._**

* Indenting and same line perform the same way. For example:

```python
# These two lines perform the same way

# Format 1: Two lines
if x > 5:
  print "X is greater than five."

# Format 2: One line
if x > 5: print "X is greater than five."
```

* Conditional statements are performed as long as indenting is shown. Maintain indentation to indicate the scope of the block (which lines are affected by the `if`/`for`). Reduce indent to indicate the end of the block. For example:

```python
# Set x equal to 5
x = 5

# This line of code will run if the condition is true
if x = 5:
  print "The conditional statement is running."
  print "x is equal to 5."
  print "End of conditional statement."

# This line of code will run regardless, since it is not indented
print "Done."
```

### Nested Decisions

```python
x = 42

# Nested Conditional Statement
# Another conditional statement may run after the first if it is true.
if x > 1:
  print: 'More than one'
  if x < 100:
    print 'Less than 100'

# End of script    
print 'Done.'
```
### Two Way Decisions

```python
x = 4

# Two Way Decision
# Only one is executed in the statement
if x > 2:
  print 'Bigger'
else:
  print 'Smaller'

print 'Done.'
```

### Multi-Way Decisions

```python
# Multi-Way Decision
# Only one is executed, but there are three, or more, options that can be run.
if x < 2:
  print: 'Small'
elif x < 10: # elif stands for 'else/if'
  print: 'Medium'
else:
  print: 'Large'
print: 'Done.'
```
Notes:
* The `else` statement isn't needed while running a multi-way decision conditional statement.
* You can list many (no limit) of `elif` statements in a conditional statement.

### Try and Except Structure
* Surround a *dangerous section* of code with `try` and `except`.
* If the code in `try` works, the `except` is skipped.
* If the code in `try` fails, it runs to the `except` section.

For example:
```python
stringInput = 'Bob' #Input in a string variable

# Try the following statement
try:
  changeToInteger = int(stringInput) #Try to change the input to an integer
# If the try statement can't be executed, run the following code
except:
  changeToInteger = -1

print 'Done.', changeToInteger
```

```python
userInputString = raw_input('Enter a number:')

try:
  integerChange = int(userInputString)
except:
  integerChange = -1

if integerChange > 0:
  print 'Success!'
else:
  print 'Not a number, please enter a valid number.'
```

### Chapter Quizzes
*Problem:* Write a program to prompt the user for hours and rate per hour using `raw_input` to compute gross pay. Pay the hourly rate for the hours up to 40 and 1.5 times the hourly rate for all hours worked above 40 hours. Use 45 hours and a rate of 10.50 per hour to test the program (the pay should be 498.75). You should use `raw_input` to read a string and `float()` to convert the string to a number. Do not worry about error checking the user input - assume the user types numbers properly.

*Solution:*
```python
# Ask the user to input the number of hours worked and their hourly pay rate.
hoursInput = raw_input("Enter Hours:")
payInput = raw_input("Enter Hourly Pay:")

# Convert the strings to floats
hoursFloat = float(hoursInput)
payFloat = float(payInput)

# If the worker worked 40 hours or less, pay them their hourly rate
if hoursFloat <= 40:
    grossPay = (hoursFloat * payFloat)
# Else if the worker worked over 40 hours, pay them 1.5 times their hourly rate beyond their 40 hour work week.
elif hoursFloat > 40:
    overtimeHrs = hoursFloat - 40
    grossPay = (40 * payFloat) + (overtimeHrs * (payFloat * 1.5))
# Print the gross pay for the employee
print grossPay
```

*Problem:* Rewrite your pay program using `try` and `except` so that your program handles non-numeric input gracefully.

*Solution:*
```python
# Ask the user to input the number of hours worked and their hourly rate
hoursInput = raw_input("Enter Hours:")
payInput = raw_input("Enter Hourly Pay:")

# Try to convert the strings to floats
try:
  hoursFloat = float(hoursInput)
  payFloat = float(payInput)
# If anything fails during the 'try', run the following error message, and quit.
except:
  print "Error, please enter numeric input."
  quit()
# If the worker worked 40 hours or less, pay them their hourly rate
if hoursFloat <= 40:
  grossPay = (hoursFloat * payFloat)
# Else if the worker worked over 40 hours, pay them 1.5 times their hourly rate beyond their 40 hour work week.
elif hoursFloat > 40:
  overtimeHrs = hoursFloat - 40
  grossPay = (40 * payFloat) + (overtimeHrs * (payFloat * 1.5))
# Print the gross pay for the employee
print grossPay
```

*Problem:* Write a program to prompt for a score between 0.0 and 1.0. If the score is out of range, print an error. If the score is between 0.0 and 1.0, print a grade using the following table:

| Score    | Grade    |
| :------------- | :------------- |
| >= 0.9        | A       |
| >= 0.8      | B       |
| >= 0.7      | C     |
| >= 0.6      | D      |
| < 0.6      | F      |


If the user enters a value out of range, print a suitable error message and exit. For the test, enter a score of 0.85.

*Solution:*
```python
# Ask the user to enter their score
scoreInput = raw_input("Enter your score (0.0 - 1.0):")

# Try to convert to a float.
try:
    scoreFloat = float(scoreInput)
# If it fails, run an error message, and quit.
except:
  print "Error, please enter a score between 0.0 and 1.0."
  quit()

# Show the user their grade, unless the number is greater than 1.0
if scoreFloat <= 1.0:
  if scoreFloat >= 0.9:
      print "A"
  elif scoreFloat >= 0.8:
      print "B"
  elif scoreFloat >= 0.7:
      print "C"
  elif scoreFloat >= 0.6:
      print "D"
  elif scoreFloat < 0.6:
      print "F"
else:
  print: "Error, please enter a score between 0.0 and 1.0."
```
## Chapter 4: Functions
Functions are reusable code that takes arguments as input, does computation, and returns a result(s). This is the **store** and **reuse** pattern.

### What are Functions
* Functions work as such: **Argument → Parameter → Result**
* Defined using the `def` reserved word.
* Called/invoked by using the function name, parenthesis, and arguments in an expression.
* Create a function if something gets too long or too complex. Break it up into logical chunks and put each chunk into a function.

For example:
```python
def hello():
  print "Hello there!"
  print "Python rocks!"

print "Running the hello function..."
hello()
print "...The hello function is done."
```

As a result the following will print on the screen:
```
Running the hello function...  
Hello there!  
Python rocks!  
...The hello function is done.
```

### Types of Functions

* **Built-in Functions:** Provided as part of Python (e.g. `raw_input()`, `type()`, `float()`, `int()`, etc.)

* **Defined Functions:** Functions defined by us using the `def` keyword. Defining the function does not execute it, it is only defined.

### Arguments
An argument is a value passed into a function as its input when calling the function. They are placed in parenthesis after the name of the function.

Arguments are used to direct the function to do different kinds of work at different times.

*Multiple arguments can exist in a function.*

For example: In the example below `Hello world` is the argument.
```python
# Arguments pass into the function
big = max('Hello world')
```

### Parameters
A variable used in a function definition that is a "handle" allowing code in the function to access the arguments for a particular function invocation. *Multiple parameters can exist within a function.*

For example:
```
# In this example, 'languageSpoken' is the parameter
def greetingText(languageSpoken)
  if languageSpoken == 'es':
    print 'Hola'
  elif languageSpoken == 'fr':
    print 'Bonjour'
  else:
    print 'Hello'

# The responses after running the arguments through the parameter.
>> greetingText('en')
Hello

>> greetingText('es')
Hola

>> greetingText('fr')
Bonjour
```

### Return Values
A function will take its arguments, do computations, and return a value to be used as the value of the function call in the calling expression. The return keyword is used for this.

For example:
```python
def greeting():
  return "Hello,"

print greet(), "Professor Snape"
print greet(), "Harry Potter"
```

Will Return:
```
Hello, Professor Snape
Hello, Harry Potter
```
Another example:
```
def greetingText(languageSpoken)
  if languageSpoken == 'es':
    print 'Hola'
  elif languageSpoken == 'fr':
    print 'Bonjour'
  else:
    print 'Hello'

# The responses after running the arguments through the parameter with return values
>> greetingText('en'), Harry
Hello Harry

>> greetingText('es'), Hermoine
Hola Hermoine

>> greetingText('fr'), Ron
Bonjour Ron
```
### Void Functions
A function doesn't have to have a return value, also known as "not fruitful".

### Chapter Quiz
*Problem:* Write a program to prompt the user for hours and rate per hour using `raw_input` to compute gross pay. Award time-and-a-half for the hourly rate for all hours worked above 40 hours. Put the logic to do the computation of time-and-a-half in a function called `computepay()` and use the function to do the computation. The function should return a value. Use 45 hours and a rate of 10.50 per hour to test the program (the pay should be 498.75). You should use `raw_input` to read a `string` and `float()` to convert the `string` to a `number`. Do not worry about error checking the user input unless you want to - you can assume the user types numbers properly.

*Solution:*
```python
# Define the computePay function
def computePay(hours,rate):
    # If the worker worked over 40 hours, pay them 1.5 times their hourly rate.
    if hoursFloat > 40:
        overtimeHours = hours - 40
        return (40 * rate) + (overtimeHours * (rate * 1.5))
    # If the worker worked 40 hours or less, pay them their hourly rate.
    elif hoursFloat <= 40:
        return (hours * rate)

# Ask the user to input the number of hours worked and their hourly rate.
inputHours = raw_input("Enter Hours:")
inputRate = raw_input("Enter Hourly Rate:")

#Convert the strings to floats
hoursFloat = float(inputHours)
rateFloat = float(inputRate)

# Run the function
totalPay = computePay(hoursFloat,rateFloat)

# Print the gross pay for the employee
print totalPay
```
## Chapter 5: Loops and Iteration
Looping, or repeated steps, have iteration variables that change each time through a loop. Often these iteration variables go through a sequence of numbers.

### Indefinite Loop
Also known as `while` loops, because they keep going until a logicial condition becomes false.

For example:
```python
n = 5
# Run this following code while it remains true
while n > 0:
  print n
  n = n - 1
# The end of the loop
print "Done!"
print n
```

Which will show the following output:
```
5
4
3
2
1
Done!
0
```

### Definite Loop
A list of items, effectively a finite set of things using the `for` construct. Definite loops are executed an exact number (explicit iteration values) of times as they iterate through the members of a sequence/set.

Quite often we have a list of items, effectively a finite set of things where a definite loop is the best solution.

For example:  
```python
# Run this code for a specific amount of iterations as-defined
for i in [5,4,3,2,1]:
  print i
print 'Done.'
```

Will show:
```
5
4
3
2
1
Done.
```

```python
# You can run a definite loop with strings as well!
friends = ['Joseph','Glenn','Sally']

for friend in friends:
  print 'Happy New Year:', friend
print 'Done.'
```

Will show:
```
Happy New Year: Joseph
Happy New Year: Glenn
Happy New Year: Sally
Done.
```

### ~~Infinite Loop~~
Avoid using infinite loops, they will continue to run! For example:

```python
# This loop will never end as n will always be greater than 0.
n = 5
while n > 0:
  print 'Lather'
  print 'Rinse'
print 'Dry off!'
```

### ~~Zero Loop~~
Try to avoid zero loops, or a loop that will never run. For example:

```python
n = 0
# This loop will never run as n is already 0
while n > 0:
  print 'Lather'
  print 'Rinse'
print 'Dry off!'
```
### Breaking Out of a Loop
The `break` statement ends the current loop and jumps to the statement immediately following the loop. For example:

```python
while True:
  line = raw_input('>')
  # If the user enters in 'done', leave the loop
  if line == 'done':
    break
    print line
print 'Done!'
```

If the user types the following, this will be the response:
```
> hello there
hello there
> finished
finished
> done
Done!
```
### Finish an Iteration with `continue`
The `continue` statement ends the current iteration and jumps to the top of the loop and starts the next iteration. For example:

```python
while True:
  line = raw_input('>')
  if line[0] == '#':
    continue
  if line == 'done':
    break
  print line
print 'Done!'
```
Where:
```
> hello there
hello there
> # don't print this
> print this!
print this!
> done
Done!
```

### Looking at `In`
<img width="957" alt="screen shot 2015-10-05 at 6 02 38 pm" src="https://cloud.githubusercontent.com/assets/5023024/10296134/536a9b50-6b8b-11e5-8bd2-444f02d45b80.png">

### Making Smart Loop Idioms
This trick is "knowing" something about the whole loop when you are stuck writing code that only sees one entry at a time (**the before, during, and after**).
* Set variables to initial values.
* For the thing in the data look for something to each entry separately, updating a variable.
* Look at the variables (the payoff).

For example, finding the largest number:
```python
largestSoFar = -1
print 'Before', largestSoFar
for theNum in [9,41,12,3,74,15]:
  if theNum > largestSoFar:
    largestSoFar = theNum
  print largestSoFar, theNum

print 'After', largestSoFar
```

The results are as follows:
```
$python largest.py
Before -1
9 9
41 41
41 12
41 3
74 74
74 15
After 74
```

Another example, finding the smallest number:
```python
# Set smallest to none to give it no value
smallest = None
print 'Before'
for value in [9,41,12,3,74,15]:
  # If smallest is still none, set the value as smallest.
  if smallest is None:
    smallest = value
# Else if the value is smaller than the smallest value, make the new value the smallest value.
  elif value < smallest:
    smallest = value
  print smallest, value

print 'After',smallest
```

The results are as follows:
```
$python smallest.py
Before
9 9
9 41
9 12
3 3
3 74
3 15
After 3
```
### The `is` and `is not` operators
* `Is` and `is not` can be used in logical expressions.
* Implies 'is the same as'
* Similar to, but stronger than `==`
* **Do not** use in most circumstances, only recommended uses are for `none`, `true`, and `false`.

For example:  
```python
if smallest is None
```

### Chapter Quiz
*Problem*: Write a program that repeatedly prompts a user for integer numbers until the user enters 'done'. Once 'done' is entered, print out the largest and smallest of the numbers. If the user enters anything other than a valid number catch it with a `try`/`except` and put out an appropriate message and ignore the number. Enter the numbers from the book for problem 5.1 and Match the desired output as shown.

*Solution*:
```python
# Set the largest and smallest numbers to None by default
largest = None
smallest = None

# While loop
while True:
    # User input to enter a number
    input = raw_input("Enter a number: ")
    # If the user enters 'done', leave the loop
    if input == "done" : break
    # Try to convert the number to an integer
    try:
        number = int(input)
    # If the conversion doesn't work, throw an error handler
    except ValueError:
        print "Invalid input"
    else:
        # If smallest is still none, set the number to the smallest and largest numbers
        if smallest is None:
            smallest = number
            largest = number
        # Else if the number is smaller than the smallest number, set it to the smallest number
        elif number < smallest:
            smallest = number
        # Else if the number is larger than the largest number, set it to the largest number
        elif number > largest:
            largest = number
# Print the maximum and minimum numbers
print "Maximum is", largest
print "Minimum is", smallest
```
