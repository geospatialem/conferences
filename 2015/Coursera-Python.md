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
