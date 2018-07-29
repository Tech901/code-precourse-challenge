# Code 1.0 Precourse Challenge

**Objective**: A simple programming assignment suitable for a novice, yet
challenging enough to inspire confidence.

This assignment is intended to introduce some concepts of computer programming
without worrying too much about a deep knowledge of a programming language.
This will put a candidate's mind in the right place as they prepare for the
Code 1.0 course. If you are intimidated at first, you don’t need to be. This
is a very doable task for an absolute beginner! While this task is designed for
a beginner, it should be challenging enough that you will have a sense of
satisfaction and accomplishment once you've completed the assignment.

The challenge will be written in Python using the CS50 IDE (Integrated
Development Environment). This assignment is not intended to make you a Python
programmer and as such only a very small subset of the Python language will be
used. You will complete this challenge using simple tools that are native to
Python with no extended classes, libraries, or utilities.

If you are new to Python, you may want to resist the urge to delve too deeply
into the language at first. We are using it here because it is relatively easy
to write simple scripts without deep knowledge of the language. Python is a
very rich and powerful programming language used by many software professionals.
It is not necessary for you to explore Object Oriented Programming or any of
the other great features that make Python popular. For this challenge we will
steer you towards a simple subset of the language that will allow you to be
successful. A programmign tutorial is included to help you with the challenge.
If you struggle, the tutorial contains all the information necessary to be
successful.

After you complete the assignment, if you're interested in learning more, I
encourage you to explore Python as completely as you desire.  Remember though,
the primary language you will use for the majority of Code 1.0 class is "C".
You might consider expending any extra effort in that direction now and wait to
explore Python in depth later when it is addressed towards the end of the course.

Because this challenge is both to prepare you for the course and give us an idea
of your initial preparedness, it is vital that you not share the results or code
that you create with others. Let them enjoy the reward of discovery for themselves.
Likewise we expect you to perform this challenge for your own learning benefit
and on your honor not to seek or accept other's work to submit in your name.
To do so will defeat the intent and learning opportunity of this assignment.

Directions for signing up and using the CS50 IDE with Python may be found in
chapter 1 of the Code 1.0 pre-course challenge tutorial.

A Python reference and other information including tutorials can be found at
[python.org](http://www.python.org) and many other placeds all over the web.

All files required for the challenge including the `Secret.in` file and an ASCII
table PDF will be provided during the tutorial.

You may request support from Tech901 technical resources via email at this address:
[code1support@tech901.org](mailto:code1support@tech901.org).


## The challenge specifications and requirements

With cyber security issues so prevalent in the news and workplace, file
encryption has become an important skill for software developers. An encrypted
file, named `Secret.in` is included with this tutorai. Your assignment is to
write a program that will read and decrypt this file, and then write its
decrypted text into a file called `Results.out`. Your program will then append
your email address in encrypted form to the results file to be turned in for
review. A very simple and direct hash algorithm was used to encrypt the
`Secret.in` file as follows:

1. Each character of the original clear text data was hashed by converting the
   character to an integer representing that character from the ASCII table.
2. A constant value of 128 was added to that integer.
3. The resulting value was `XOR`’ed with the integer 99.
4. The final resulting integer was converted into a three-character string value
   and written into the `Secret.in` file. Each three character string is written
   sequentially from beginning to end so that the first three numbers in the file
   represent the first character of the message, the next three represent the
   second character of the message and so on.

In order to achieve success, you must write a Python script in the CS50 IDE
to decrypt the secret by reversing the hash process described above. You must
add a carriage return--`chr(12)`--to the end of the decoded text and then also
use the original hash procedure as described above to write your encrypted email
address to the end of the results file.  Once you have configured your
environment this should only take a few hours to complete.  Don’t worry if you
struggle at first.  Take it one step at a time.  If you need help, use the email
address for support. **YOU CAN DO THIS!**

You will need to become familiar with the following elements of the Python
language for the project:

- File I/O,
- Variable types (especially int, chr, and str),
- Variable type conversion,
- Boolean functions (XOR),
- Loops.

If you find yourself in other areas you may be making it too hard!

You may review your results by opening the files in the CS50 IDE editor or any
other text editor (such as notepad on Windows). When you have completed the
challenge, save your script as `precourse.py` and attach it along with your
`Results.out` file to an email with the subject: "*Code1.0 Pre-Course Assignment
Results*" and send it to [code1support@tech901.org](mailto:code1support@tech901.org).
Please feel free to comment on the challenge and your method for completing it.

Good luck with the assignment and we look forward to your success with Code 1.0
and your new career as a software developer!


## Let's get started!

Continue to the [Tutorial](tutorial.md)!
