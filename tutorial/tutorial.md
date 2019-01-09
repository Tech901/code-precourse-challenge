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

1. Chapter 1. [Sign Up with CS50 edX and set up your IDE environment](#chapter-1-sign-up-for-cs50)
2. Chapter 2. [Python Language Syntax (code formatting rules)](#chapter-2-python-language-syntax)
3. Chapter 3. [Python data and variables (numbers, letters, and such)](#chapter-3-python-data-and-variables)
4. Chapter 4. [Python operators](#chapter-4-python-operators)
5. Chapter 5. [Flow Control with the If statement (If this is true then do that, otherwise do something else)](#chapter-5-if-statements)
6. Chapter 6. [Python Loops (how to repeat something multiple times)](#chapter-6-loops)
7. Chapter 7. [Python File I/O (Input(reading from) / Output (writing to) a file)](#chapter-7-file-io)
8. Chapter 8. [Python conversion functions (How to change letters to numbers and such)](#chapter-8-conversion-functions)
9. Chapter 9. [ASCII table (numbers that represent letters)](#chapter-9-ascii-table)
10. Chapter 10. [Hashing and Encryption (How to decode and encrypt data)](#chapter-10-hashing-and-encryption)
11. Chapter 11. [The Secret.in file format (you will read from this)](#chapter-11-the-secretin-file)
12. Chapter 12. [The Results.out file format  (you will write to this)](#chapter-12-the-resultsout-file)
13. Chapter 13. [A Step-by-step guide](#chapter-13-a-step-by-step-guide)
14. Chapter 14. [Sending your results to us (and gloating about your success)](#chapter-14-sending-your-results-to-us)


## Chapter 1: Sign up for CS50

Much of the Code 1.0 course follows Harvard's CS50 curriculum. Additionally,
we'll use the online CS50 IDE environment to write and run our code.

To get started, [Enroll in the the CS50x course at edX.org](https://www.edx.org/course/introduction-computer-science-harvardx-cs50x).



**TODO** this section is incomplete... more content coming soon.


### A brief tour of the CS50 IDE

The programming environment that we will throughout this course is called the
CS50 IDE. It's a web-based programming environment, and should work well on any
modern computer: Macs, PCs running Windows or Linux, and even Chromebooks.

![The CS50 IDE](images/CS50_IDE.jpg)

There are three main sections of the CS50 IDE:

1. The **File Pane** lists the files and directories in your workspace.
2. The **Editor** is a text editor; this is where we will write much of our code.
3. The **Terminal** gives you access to a Linux command line.

If you accidentally close the Editor or Terminal, you can always reopen them.
If your CS50 IDE looks different from the screenshot above, never fear! You
still have access to all the tools.

Here's how you'd open a new Terminal:

![Opening a terminal](images/opening-a-terminal.gif)


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


## Chapter 5. If statements

    TODO:  need to complete this.

## Chapter 6. Loops

## Chapter 7. File I/O

## Chapter 8. Conversion Functions

## Chapter 9. ASCII table

ASCII stands for **American Standard Code for Information Interchange**.
Computers can only understand numbers, so an ASCII code is the numerical
representation of a character such as 'a' or '@' or an action of some sort.
ASCII was developed a long time ago and now the non-printing characters are
rarely used for their original purpose(teletype machines). The original ASCII
code consisted of 128 Characters of printable and non-printable device control
codes. Each was represented by a seven bit binary code with values ranging from
decimal 0 through 127.

**Hint**: every ASCII character can be represented by a 3 digit decimal number!

The following ASCII Table shows you the convesion from a decimal valu to a
character value.

    Dec  Char                           Dec  Char     Dec  Char     Dec  Char
    ---------                           ---------     ---------     ----------
      0  NUL (null)                      32  SPACE     64  @         96  `
      1  SOH (start of heading)          33  !         65  A         97  a
      2  STX (start of text)             34  "         66  B         98  b
      3  ETX (end of text)               35  #         67  C         99  c
      4  EOT (end of transmission)       36  $         68  D        100  d
      5  ENQ (enquiry)                   37  %         69  E        101  e
      6  ACK (acknowledge)               38  &         70  F        102  f
      7  BEL (bell)                      39  '         71  G        103  g
      8  BS  (backspace)                 40  (         72  H        104  h
      9  TAB (horizontal tab)            41  )         73  I        105  i
     10  LF  (NL line feed, new line)    42  *         74  J        106  j
     11  VT  (vertical tab)              43  +         75  K        107  k
     12  FF  (NP form feed, new page)    44  ,         76  L        108  l
     13  CR  (carriage return)           45  -         77  M        109  m
     14  SO  (shift out)                 46  .         78  N        110  n
     15  SI  (shift in)                  47  /         79  O        111  o
     16  DLE (data link escape)          48  0         80  P        112  p
     17  DC1 (device control 1)          49  1         81  Q        113  q
     18  DC2 (device control 2)          50  2         82  R        114  r
     19  DC3 (device control 3)          51  3         83  S        115  s
     20  DC4 (device control 4)          52  4         84  T        116  t
     21  NAK (negative acknowledge)      53  5         85  U        117  u
     22  SYN (synchronous idle)          54  6         86  V        118  v
     23  ETB (end of trans. block)       55  7         87  W        119  w
     24  CAN (cancel)                    56  8         88  X        120  x
     25  EM  (end of medium)             57  9         89  Y        121  y
     26  SUB (substitute)                58  :         90  Z        122  z
     27  ESC (escape)                    59  ;         91  [        123  {
     28  FS  (file separator)            60  <         92  \        124  |
     29  GS  (group separator)           61  =         93  ]        125  }
     30  RS  (record separator)          62  >         94  ^        126  ~
     31  US  (unit separator)            63  ?         95  _        127  DEL

So any letter in the alphabet can be represented by a numeric value. For example,
a capital `B` is 66 while a lowercase `m` is 109.

## Chapter 10. Hashing and Encryption

A *cryptographic hash function* is a special class of [hash function](https://en.wikipedia.org/wiki/Hash_function) that has certain properties which make it suitable for use in [cryptography](https://en.wikipedia.org/wiki/Cryptography).

It is a mathematical algorithm that maps data of arbitrary size to a bit string
of a fixed size (a [hash function](https://en.wikipedia.org/wiki/Hash_function))
which is usually designed to also be a one-way function, that is, a function
which is infeasible to invert. The only way to recreate the input data from an
ideal cryptographic hash function's output is to attempt a brute-force search
of possible inputs to see if they produce a match, or use a "rainbow table" of
matched hashes. [Bruce Schneier](https://en.wikipedia.org/wiki/Bruce_Schneier)
has called one-way hash functions "the workhorses of modern cryptography".[[1](https://en.wikipedia.org/wiki/Cryptographic_hash_function#cite_note-1)].

The input data is often called the message, and the output (the hash value or
hash) is often called the message digest or simply the digest.  The hash routine
you will be using for this challenge is neither one-way nor is it difficult to
crack by serious security professionals. This hash routine is only intended to
introduce you to the concepts of obscuring sensitive data by encryption and
character data represented by transformed numeric, binary, or unreadable
characters in a file, while providing an interesting assignment to challenge
a new programmer to think about his code.

The challenge routine simply obscures the clear text data by using the following
process:

1. Converting each character of the text data into a 3 digit integer equivalent
   from the ASCII tables chr to decimal chart.
2. Adding 128 to the converted ASCII code
3. Performing an *exclusive or* operation (XOR) on each character’s ASCII code
   with the number 99.
4. Converting the integer decimal value to a 3 character string representing
   the same numeric value.
5. Writing the 3 character string values consecutively to the encrypted file
   for each character in the original clear text.

To decrypt the data again, simply perform the previous steps in exactly the
reverse order. You will know if you have successfully decrypted the file if
you produce readable text that makes some sense and does not appear jumbled.


## Chapter 11. The Secret.in file

Download the [Secret.in](Secret.in) file. There are a couple ways you can access
this file.

1. Run this command in you CS50 IDE terminal:

    wget https://raw.githubusercontent.com/Tech901/code-precourse-challenge/master/tutorial/Secret.in

2. You can download the file to your local computer, then drag &amp; drop it
   into the CS50 IDE:


![Upload Secret.in to CS50 IDE](images/uploading-secret-file.gif)


This file contains the encrypted information that you must decode. If you open
it in notepad (or any other text editor) it looks like rows and rows of numbers.
The secret text you are trying to decode is hidden from plain view by encoding
the letters of the text into numbers so that they cannot be read without
decoding them with the same routine that was used to encode them.

In the `Secret.in` file, each letter, space, and punctuation are represented by
a 3-digit code. The first 3 numbers, 183, represent the first letter of the message.
The next 3 numbers, 139, represent the next letter, and so on and so on through
the end of the file. In the chapter on [Hashing and Encryption](#chapter-10-hashing-and-encryption),
we explained how to decode these numbers so that the secret text can be read.
**Be careful not to save over or modify the `Secret.in` file as that could
scramble the code.** If you think you may have altered it, you can always download
it again.

## Chapter 12. The Results.out file

The `Results.out` file is a file that will be created by the Python program you
write. It will contain the results from your program so that we can determine if
you have successfully completed the assignment. The first part of the file will
contain the decoded secret message in clear text that can be directly read in
notepad or any file viewer (such as the CS50 IDE's editor). After the full clear
text of the secret message, a coded signature message will follow. This will be
your email address encoded with the same cipher routine that was used to code the
original `Secret.in` file that you decoded.

When we check your `Results.out` file, we should see the decoded secret message
in clear text, followed by a series of 3 digit numbers. When we decode that message,
we should see your email address.

## Chapter 13. A Step-by-step guide

## Chapter 14. Sending your results to us


Once you have completed the assignment and created the `Results.out` file,
create an email and attach your `Results.out` file and your `precourse.py` file.

Send the email to: [mailto:Code1support@tech901.org](Code1support@tech901.org).
The subject line should say “Code1.0 Pre-Course Assignment Results.out”. In the
body of the email please tell us what you thought of the assignment and give us
any constructive suggestions to improve it. We'd also love to hear how you
solved the challenge and if you needed the step by step tutorial or not.


**Good Luck!**
