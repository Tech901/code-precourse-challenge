# Code 1.0 Precourse Challenge

This tutorial is intended to explain how to complete the Code 1.0 cyber security
challenge. It is not, however, a fully-complete tutorial on the Python language.
For simplicity, this tutorial will guide you through one possible path to the
solution. We have pulled together all the information you need in this document.

More complex concepts which may have taken more time to explain and comprehend
have been ignored or avoided. You will be expected to learn languages at a
deeper level during the Code 1.0 class, but for now we’ll keep it simple. There
is no reason for you not to succeed with this challenge, even if you are a
complete beginner, if you follow this guide.

**You can do this!**

## Contents

1. Chapter 1. Sign Up with CS50 edX and set up your IDE environment.
2. Chapter 2. Python Language Syntax (code formatting rules)
3. Chapter 3. Python data and variables (numbers, letters, and such)
4. Chapter 4. Python operators
5. Chapter 5. Flow Control with the If statement (If this is true then do that, otherwise do something else)
6. Chapter 6. Python Loops (how to repeat something multiple times)
7. Chapter 7. Python File I/O (Input(reading from) / Output (writing to) a file)
8. Chapter 8. Python conversion functions (How to change letters to numbers and such)
9. Chapter 9. ASCII table (numbers that represent letters)
10. Chapter 10. Hashing and Encryption (How to decode and encrypt data)
11. Chapter 11. The Secret.in file format (you will read from this)
12. Chapter 12. The Results.out file format  (you will write to this)
13. Chapter 13. Sending your results to us (and gloating about your success)
14. Glossary -  Terms you may want or need to be familiar with…


## Chapter 1: Sign up for CS50

Much of the Code 1.0 course follows Harvard's CS50 curriculum. Additionally,
we'll use the online CS50 IDE environment to write and run our code.

To get started, [Enroll in the the CS50x course at edX.org](https://www.edx.org/course/introduction-computer-science-harvardx-cs50x).



**NOTE** this section is incomplete... more content coming soon.


## Chapter 2. Python Language Syntax

Python is an extremely powerful language with many attributes and capabilities
that many appreciate when contrasted to other computer languages. In addition,
Python also contains an interactive interpreter which allows immediate commands
to be entered with actions performed and results displayed in real time.
It is for that reason that we chose it as a simple and effective tool to introduce
the concept of computer programing. Our examples will utilize the CS50 IDE and
the Python interactive command interpreter window it provides.

_Syntax_ is defined as “the arrangement of words and phrases to create well-formed
sentences in a language.”  In the case of computer science, the syntax of a
computer language is the set of rules that defines the combinations of symbols
that are considered to be a correctly structured document or fragment in that
language.

Python statements have a particular order and format to them that the Python
interpreter can process. All computer languages have their own specific syntax.
If you format a statement incorrectly Python will respond with an error.
You will have to correct the syntax in order to continue.

### Python Comments

When working with any programming language, you include comments in the code to
notate your work. This helps explain portions of your code, and lets other
developers – you included – know what you were thinking when you wrote the code.
This is a necessary practice, and good developers using comments wisely.

### How to Write Comments in Python

In Python, there are two ways to annotate your code. The first is to include
comments that detail or indicate what a section of code – or snippet – does.
The second makes use of multi-line comments or paragraphs that serve as
documentation for others reading your code.

Think of the first type as a comment for yourself, and the second as a comment
for others. There is no right or wrong way to add a comment, however. You can
do whatever feels comfortable.

Single-line comments are created simply by beginning a line with the hash
character (a `#`), and they are automatically terminated by the end of line.
This type of comment is called an _inline comment_. For example:

    # This would be a comment in Python

A Comment that spans multiple lines – used to explain things in more detail –
are created by wrapping the comments in triple-quotes (either `'''` or `"""`).
These are known as _docstrings_:

    '''This would be a multiline comment
    in Python that spans several lines and
    describes your code or anything you want it to.
    '''

Remember to comment as often as possible. It's important! Python has no
mandatory statement termination characters and blocks are specified by
indentation. Indent to begin a block, dedent to end one. Statements that
expect an indentation level end in a colon (:).  We’ll see some specific
examples later.


## Chapter 3. Python data and variables

Computer languages including Python work with and manipulate data in various
forms such as numbers and text. Variables are used to name and temporarily store
data while the computer is processing or performing actions on it. You can think
of variables as a box or container for pieces data. Every variable has a name
and a type.

The variable name is a descriptive label used to work with that particular storage
container (a location in the computer's memory) of data. Every variable has a
“type” which describes the type or nature of the data in the container.  A
variable that contains just number values is a different “type” than one that
contains text number characters or letters.

Python is a strongly typed (i.e. types are enforced), dynamically, implicitly
typed (i.e. you don't have to declare variables), case sensitive (i.e. var
and VAR are two different variables).  This means that when you use a variable,
Python automatically looks at the data you are storing and if it is a number
value, assigns it the correct type.

Values are assigned to variable names with the assignment operator, the equals
sign (`=`).  So you can write code like:

    a = 3

Python will determine that 3 is an integer and store it in a variable named `a`
as an integer type. You can use `a` to add, `a = a + 2`, or use the python
shorthand `a +=2`, or you can perform other mathematical operations because it
is an integer type. In both of the previous examples, the variable `a` would
contain the value 5.

You can assign text to a variable by writing something like:

    message = "Hello"

Python again automatically recognizes that "Hello" is text data and assigns the
variable names `message` with the type `str` or string. You can add or
concatenate more text to message by writing:

    message = message + " world"

Now, the variable `message` would contain the data “Hello world” (notice the
space in front of `" world"`). But if you attempted to add an integer value
(e.g. `message = message + 5`), python would raise an Exception (or an error).

Variable names can be almost any continuous string of characters long or short.
It is always good practice to make variable names meaningful to describe the
data or value they contain. For instance if you were writing a program for an
automotive use and needed to store the pressure of air in a tire, you could name
the variable `a`, `t`, or `tire_pressure`. All are valid variable names, but
only one is self-descriptive. Can you guess which one!? Later in a very complex
program it would be more meaningful if the variable name let you know at a
glance what information it represented.

Python defines many different data types. We will only concern ourselves with a
few simple types you will need to perform this challenge, Numbers and Strings.

### Python Numeric types

Numeric data types store numbers. Number objects are created when you assign a
value to them. For example:

    var1 = 1
    var2 = 10


Python supports three [numeric types](https://docs.python.org/3/library/stdtypes.html#numeric-types-int-float-complex):

- `int` (integers)
- `float` (floating point or decimal values)
- `complex` (complex numbers have a *real* and *imaginary* component; We
  won't use them in this tutorial)


Here are some examples of numbers:

| int            | float   |
|----------------|---------|
| 10             | 0.0     |
| 100            | 15.20   |
| -786           | -21.9   |
| -4721885298529 | 32.3e18 |

### Strings

Strings in Python are identified as a contiguous set of characters represented
in quotation marks. Python allows for either pairs of single or double quotes,
and you can have quotation marks of one kind inside a string that uses the other
kind (i.e. `"He said 'hello'."` is valid).

The plus (`+`) sign is the string concatenation operator and allows you to add
strings together to create longer strings. The asterisk (`*`) is the repetition
operator and will create multiple copies of the string. Equality testing is done
using two equals signs (`==`).

Subsets or parts of strings can be taken using the **indexing** and **slice**
operator (`[]` and `[:]`). An index is a kind of pointer to a particular
location in the string, starting at 0. In Python the first character location
or index is always 0 and not 1. You might need to use the subset slice operator
soon (hint hint)!

Here are some examples.


    message = 'Hello World!'
    print (message)          # Prints the complete string
    print (message[0])       # Prints first character of the string
    print (message[2:5])     # Prints characters starting from 3rd to 5th
    print (message[2:])      # Prints a subset of the string starting from the 3rd character
    print (message * 2)      # Prints the string two times
    print (message + "TEST") # Prints concatenated strings

The above code would produce the following results:

    Hello World!
    H
    llo
    llo World!
    Hello World!Hello World!
    Hello World!TEST

You can try this for yourself in the CS50 IDE! To launch a python interpreter,
find the terminal window, and at the `$` prompt, type `python`. At this point,
you should see a `>>>` prompt. This is the python prompt; You are now working
with a python interactive shell. Type:

        str  = "Hello World!"

Then to print the string, you can write the following code (NOTE: you don't have
to type the `>>>`, but you should see them on your screen).

     >>>  print(str)

Try each of the commands in the example above.

## Chapter 4. Python Operators

Operators are the constructs which can manipulate the value of operands.
Consider the expression: 4 + 5 = 9. Here, 4 and 5 are called operands and + is
called an operator.

### Types of Operators

Python supports the following types of operators.

- Arithmetic Operators
- Comparison (Relational) Operators
- Assignment Operators
- Logical Operators
- Bitwise Operators

#### Python Arithmetic Operators

Assume the variable `a` contains the value 10 and the variable `b` contains
the value 20, then:

| Operator           | Description                                          | Example | Result |
|--------------------|------------------------------------------------------|---------|-----|
| `+` Addition       | Adds values on either side of the operator.          | `a + b` | 30  |
| `-` Subtraction    | Subtracts right hand operand from left hand operand. | `a – b` | -10 |
| `*` Multiplication | Multiplies values on either side of the operator     | `a * b` | 200 |
| `/` Division       | Divides left hand operand by right hand operand      | `b / a` | 2   |

#### Comparison Operators

These operators compare the values on either sides of them and decide the relation
among them. They are also called Relational operators.

Assume variable `a` contains the value 10 and variable `b` contains the value 20, then:

- `==` **Equality**: If the values of two operands are equal, then the expression
  is true. `a == b` is not true.
- `!=` **Not Equal**: If values of two operands are not equal, then the
  expression is true. `a != b` is true.
- `>` **Greater than**: If the value on the left is greater than the value on
  the right, then the expression is true. `a > b` is not true.
- `<` **Less than**: If the value on the left is less than the value on the right,
  then the expression is true: `a < b` is true.
- `>=` **Greater than or equal to**: If the value on the left is greater than
  or equal to the value on the right, then the expression is true. `a >= b` is not true.
- `<=` **Less than or equal to**: If the value on the left is less than or equal
  to the value on the right, then condition becomes true. `a <= b` is true.

#### Assignment Operators

You've already seen how the `=` assignment operator can be used, but python also
has some *compound assignment* operators. These are simply shorthand for common
arithmetic operators, as you'll see below.

Assume variable `a` contains the value 10 and variable `b` contains the value 20, then:

- `=` **Assignment**: Stores the value in the right in the variable on the left,
  e.g. `a = 10` or `b = 20`.
- `+=` **Compound add**: Adds the value on the right to whatever is current stored
  in the variable and replaces that result in the variable. e.g. `a += 5` would
  result in `a` containing the value 15. This is the same as: `a = a + 5`.
- `-=` **Compound subtract**: Similar to compound addition, `a -= 3` would result
  in `a` containing the value 7. This is the same as `a = a - 3`.
- `*=` **Compound multiplication**: `a *= 5` would result in
  `a` containing the value 50. This is the same as: `a = a * 5`
- `/=` **Compound division**: `a /= 2` would result in `a` containing the value
  5, which is the same as `a = a / 2`.


#### Bitwise Operators

The bitwise operator works on bits (binary digits, i.e. 1 and 0) and performs
bit by bit operation. Each character or byte of data is made up of a group
(usually 8) bits. The bits are ordered so that each position represents binary
data where the only valid values are 0 and 1s. Each of these are added together
according to their position order to make up 8 bit values from 0 to 255. The
operations below compare the bit positions individually between a and b and
utilize the operation indicated by the operator to create a resulting bit
sequence. In the examples below, the "logical and" `&` operator only evaluates
as true. Assume `a = 60` and `b = 13`. These values are expressed in binary
format below:

    a = 0011 1100
    b = 0000 1101

The result of various bitwise operators are expressed below.


**Bitwise And** (the `&` operator) returns a 1 if both values are equal to 1.
Otherwise it returns a 0.

    a   = 0011 1100
    b   = 0000 1101
    -----------------
    a&b = 0000 1100


**Bitwise OR** (the `|` operator) returns a 1 of _either_ value contains a 1,
otherwise it returns a 0.

    a   = 0011 1100
    b   = 0000 1101
    -----------------
    a|b = 0011 1101


**XOR or Exclusive OR** (the `^` operator) will copy the bit if it is set in
one operand but not both. **HINT** this is important!

    a   = 0011 1100
    b   = 0000 1101
    -----------------
    a^b = 0011 0001


**Binary Ones Complement** (the unary `~` operator) has the effect of "flipping"
bits, or swapping from 0 to 1 or from 1 to 0.

    a  = 0011 1100
    ~a = 1100 0011

