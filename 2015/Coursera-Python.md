# Python for Everybody Specialization

<img src="https://d1qb2nb5cznatu.cloudfront.net/startups/i/430131-86c4ecea8ec200688933e639f890bf6d-medium_jpg.jpg?buster=1433271718" width="25" height="25">  Learn to Program and Analyze Data with Python. Develop programs to gather, clean, analyze, and visualize data.

**Courses include:**

1. **[Programming for Everybody Getting Started with Python](#1-programming-for-everybody-getting-started-with-python)**
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

### Chapter Quiz
*Problem:* Write a program to prompt the user for hours and rate per hour using `raw_input` to compute gross pay. Pay the hourly rate for the hours up to 40 and 1.5 times the hourly rate for all hours worked above 40 hours. Use 45 hours and a rate of 10.50 per hour to test the program (the pay should be 498.75). You should use `raw_input` to read a string and `float()` to convert the string to a number. Do not worry about error checking the user input - assume the user types numbers properly.

*Solution:*
```python
# Hourly pay rate
hourlyRate = 10.5

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
