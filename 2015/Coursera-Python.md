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

#### Reserved Words:
```python
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
