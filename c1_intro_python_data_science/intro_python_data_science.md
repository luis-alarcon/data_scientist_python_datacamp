
<h1>Chapter 1: Python Basics</h1>

<h2>Lesson 1: Python Basics</h2>

<h3>Exercise 1: The Python Interface</h3>
<h4>Explanation</h4>

<p>In the Python script on the right, you can type Python code to solve the exercises. If you hit Run Code or Submit Answer, your python script (script.py) is executed and the output is shown in the IPython Shell. Submit Answer checks whether your submission is correct and gives you feedback.

You can hit Run Code and Submit Answer as often as you want. If you're stuck, you can click Get Hint, and ultimately Get Solution.

You can also use the IPython Shell interactively by simply typing commands and hitting Enter. When you work in the shell directly, your code will not be checked for correctness so it is a great way to experiment.</p>

<h4>Instructions</h4>

<ol>
    <li>Experiment in the IPython Shell; type 5 / 8, for example.</li>
    <li>Add another line of code to the Python script: print(7 + 10)</li>
    <li>Hit Submit Answer to execute the Python script and receive feedback.</li>
</ol>



```python
# Example, do not modify!
print(5 / 8)

# Put code below here
print(7 + 10)
```

    0.625
    17


<h3>Exercise 2: When to use Python?</h3>
<h4>Explanation</h4>
<p>Python is a pretty versatile language. For which applications can you use Python?</p>
<h4>IPossible Answers</h4>

<ol>
    <li>You want to do some quick calculations.</li>
    <li>For your new business, you want to develop a database-driven website</li>
    <li>Your boss asks you to clean and analyse the results of the latest satisfaction survey.</li>
    <li><b>All of the above.</b></li>
</ol>


<h3>Exercise 3: Any Comments?</h3>
<h4>Explanation</h4>
<p>Something that Filip didn't mention in his videos is that you can add comments to your Python scripts. Comments are important to make sure that you and others can understand what your code is about.

To add comments to your Python script, you can use the # tag. These comments are not run as Python code, so they will not influence your result. As an example, take the comment on the right, # Division; it is completely ignored during execution.</p>
<h4>
Instructions</h4>

<ol>
    <li>Above the print(7 + 10), add the comment # Addition.</li>

</ol>



```python
# Division
print(5 / 8)

# Addition
print(7 + 10)
```

    0.625
    17


<h3>Exercise 4: Python as a calculator</h3>
<h4>Explanation</h4>
<p>Python is perfectly suited to do basic calculations. Apart from addition, subtraction, multiplication and division, there is also support for more advanced operations such as:</p>
<ul>
    <li>Exponentiation: **. This operator raises the number to its left to the power of the number to its right. For example 4**2 will give 16.</li>
    <li>Modulo: %. This operator returns the remainder of the division of the number to the left by the number on its right. For example 18 % 7 equals 4.</li>
</ul>
<p>The code in the script on the right gives some examples.</p>
<h4>
Instructions</h4>

<ol>
    <li>Suppose you have $100, which you can invest with a 10% return each year. After one year, it's 100×1.1=110 dollars, and after two years it's 100×1.1×1.1=121. Add code on the right to calculate how much money you end up with after 7 years.</li>

</ol>



```python
# Addition, subtraction
print(5 + 5)
print(5 - 5)

# Multiplication, division, modulo, and exponentiation
print(3 * 5)
print(10 / 2)
print(18 % 7)
print(4 ** 2)

# How much is your $100 worth after 7 years?
print(100*1.1**7)
```

    10
    0
    15
    5.0
    4
    16
    194.87171000000012


<h3>Exercise 5: Variable Assignment</h3>
<h4>Explanation</h4>
<p>In Python, a variable allows you to refer to a value with a name. To create a variable use =, like this example:</p>
<ul>
<li>x = 5</li>
</ul>
<p>You can now use the name of this variable, x, instead of the actual value, 5.

Remember, = in Python means assignment, it doesn't test equality!</p>
<h4>
Instructions</h4>

<ol>
    <li>Create a variable savings with the value 100.</li>
    <li>Check out this variable by typing print(savings) in the script.</li>
</ol>



```python
# Create a variable savings
savings = 100

# Print out savings
print(savings)
```

    100


<h3>Exercise 6: Other variable types</h3>
<h4>Explanation</h4>
<p>In the previous exercise, you worked with two Python data types:</p>
<ul>
    <li>int, or integer: a number without a fractional part. savings, with the value 100, is an example of an integer.</li>
    <li>float, or floating point: a number that has both an integer and fractional part, separated by a point. factor, with the value 1.10, is an example of a float.</li>
</ul>
<p>Next to numerical data types, there are two other very common data types:</p>
<ul>
    <li>str, or string: a type to represent text. You can use single or double quotes to build a string.</li>
    <li>bool, or boolean: a type to represent logical values. Can only be True or False (the capitalization is important!).</li>
</ul>
<h4>
Instructions</h4>

<ol>
    <li>Create a new string, desc, with the value "compound interest".</li>
    <li>Create a new boolean, profitable, with the value True.</li>
</ol>



```python
# Create a variable desc
desc = "compound interest"

# Create a variable profitable
profitable = True
```

<h3>Exercise 7: Guess the type</h3>
<h4>Explanation</h4>
<p>To find out the type of a value or a variable that refers to that value, you can use the type() function. Suppose you've defined a variable a, but you forgot the type of this variable. To determine the type of a, simply execute:</p>
<ul>
    <li>type(a)</li>
</ul>
<p>We already went ahead and created three variables: a, b and c. You can use the IPython shell on the right to discover their type. Which of the following options is correct?</p>
<h4>
Possible Answers</h4>

<ol>
    <li>a is of type int, b is of type str, c is of type bool</li>
    <li>a is of type float, b is of type bool, c is of type str</li>
    <li><b>a is of type float, b is of type str, c is of type bool</b></li>
    <li>a is of type int, b is of type bool, c is of type str</li>
</ol>



```python
#variables
a = 194.87171000000012
b = "True"
c = False

print(type(a))
print(type(b))
print(type(c))
```

    <class 'float'>
    <class 'str'>
    <class 'bool'>


<h3>Exercise 8: Operations with other types</h3>
<h4>Explanation</h4>
<p>Filip mentioned that different types behave differently in Python.

When you sum two strings, for example, you'll get different behavior than when you sum two integers or two booleans.

In the script some variables with different types have already been created. It's up to you to use them.</p>
<h4>
Instructions</h4>

<ol>
    <li>Calculate the product of <code>savings</code> and <code>growth_multiplier</code>. Store the result in <code>year1</code>.</li>
    <li>What do you think the resulting type will be? Find out by printing out the type of <code>year1</code>.</li>
    <li>Calculate the sum of <code>desc</code> and desc and store the result in a new variable <code>doubledesc</code>.</li>
    <li>Print out <code>doubledesc</code>. Did you expect this?</li>
</ol>



```python
savings = 100
factor = 1.1
desc = "compound interest"

# Assign product of factor and savings to year1
year1 = savings * factor**1

# Print the type of year1
print(type(year1))

# Assign sum of desc and desc to doubledesc
doubledesc = desc + desc

# Print out doubledesc
print(doubledesc)
```

    <class 'float'>
    compound interestcompound interest


<h3>Exercise 3: Type conversion</h3>
<h4>Explanation</h4>
<p>Using the <code>+</code> operator to paste together two strings can be very useful in building custom messages.

Suppose, for example, that you've calculated the return of your investment and want to summarize the results in a string. Assuming the floats <code>savings</code> and <code>result</code> are defined, you can try something like this:</p>

<p><code>print("I started with $" + savings + " and now have $" + result + ". Awesome!")</code></p>

<p>This will not work, though, as you cannot simply sum strings and floats.

To fix the error, you'll need to explicitly convert the types of your variables. More specifically, you'll need <code>str()</code>, to convert a value into a string. <code>str(savings)</code>, for example, will convert the float savings to a string.

Similar functions such as <code>int()</code>, <code>float()</code> and <code>bool()</code> will help you convert Python values into any type.</p>
<h4>
Instructions</h4>

<ol>
    <li>Hit Run Code to run the code on the right. Try to understand the error message.</li>
    <li>Fix the code on the right such that the printout runs without errors; use the function <code>str()</code> to convert the variables to strings.</li>
    <li>Convert the variable <code>pi_string</code> to a float and store this float as a new variable, <code>pi_float</code>.</li> 
</ol>



```python
# Definition of savings and result
savings = 100
result = 100 * 1.10 ** 7

# Fix the printout
print("I started with $" + str(savings) + " and now have $" + str(result) + ". Awesome!")

# Definition of pi_string
pi_string = "3.1415926"

# Convert pi_string into float: pi_float
pi_float = float(pi_string)
```

    I started with $100 and now have $194.87171000000012. Awesome!

