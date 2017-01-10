# Python Basics 

## \(If you're familiar with Python, feel free to skip this section!\)

CodeEval, an exclusive community of over 69,000 competetive developers has assessed Python as the 'most popular coding language' for the past FIVE years \(Last Ranking - 2016\).

With such a thriving community, it's hard to come up with a reason not to get on the Python bandwagon. It's recent integration to the IBM i platform furthers the existing incentive, meaning its never been a better time to read ahead and begin your Python journey!

### Overview:

Python is a high level scripting language with object oriented features. Python offers more structure and support for large programs than shell scripts or batch files can offer while remaining a simple to use programming language. In fact, with high-level data types built in \(flexible arrays and dictionaries\) Python is actually considered a very-high-level-language. Allowing you to split your program into modules that can be reused in other Python programs greatly expands the language's inherent capabilities. Things like file I/O, system calls, sockets and even interfaces to graphical user interface toolkits can be modularized to reduce development time.  Furthermore, Python is both an interpreted language and extensible. Being an interpreted language means that no compilation and linking is necessary making it easier to experiment with features of the language. Extensibility makes it easy to add a new built-in function or module to the interpreter on an existing program and allows us to link the Python interpreter to an application written in C to use as an extension or command language for that application. Python places a strong emphasis on readability and efficiency and can be picked up easily by Java, C, Perl and other language converts.

### Installing:

The installation process is fairly straight forward if it is even needed on your system at all. Many Linux and UNIX distributions include a recent version of Python. If you enter 'python' in a command line window and you see a response from a Python interpreter, you know that you already have python installed. Otherwise you will need to download Python from [https://www.python.org/downloads/](https://www.python.org/downloads/).

### Python Odities

Before we move to the actual tutorial I thought it might be useful to list some of the language protocols that might seem foreign to new users \(as they did to me\).

##### Indentation

Python uses indentation for blocks, instead of curly praces. Both tabs and spaces are supported, but the standard indentation requires Python code to use four spaces.

```
x = 1
if x == 1:
    # indented four spaces
    print("x is 1.")
```

The above code block illustrates the use of spaces in flow-control statements such as the 'if' statement. The bottom line here is that Python recognizes spacing similar to how HTML does and misplaced or misused spaces can be fatal to program execution.

You might also note that the above code segment illustrates the lack of termination characters \(; in java\).

##### Variable Assignment

Variable definition is fairly straightforward in Python. Since it is a scripting language you can assign and reassign a variable as many times as you would like in your program. Simple operators can be executed on numbers and strings as you might expect, and Python also supports simultaneous variable assignment.

```
a, b = 3, 4
print(a, b)
```

The above code would return 3, 4 as both of the variables were assigned at once.

Furthermore, variables are dynamically typed, meaning that Python has no type declarations and instead implies them itself. Python is strongly typed however, making variable assignment and modification an important aspect of code to still be aware of even without the direct type declarations.

##### Flow Control

The last odd Python syntax we will cover is the variety of ways you can implement flow control. As an example I will use a 'while' loop with a set condition that after execution, will terminate to an 'else' statment.

```
count = 0
while (count < 5):
    print(count)
    count +=1
else:
    print("count value reached %d" %(count))
```

##### Python Interpreter \(Shell Commands\)

It should first be noted that Python utilizes an interpreter to render it's code into machine readable instructions, not a compiler. The interpreter reads in a program line by line, executing each line in order, unlike a compiler that translates the contents of the program before execution. I thought it useful to take a moment and explain the difference between the two translators as the rest of this section utilizes the Python interpreter to run simple Python commands, which can be confusing to individuals accustomed to a compiler for their code of choice.

The Python interpreter allows you to run small pieces of code in the shell and to immediately see the results. To enter the Python interpreter simply type 'python' at which point you should be brought to a new line in the shell with a &gt;&gt;&gt; at the start of the line to indicate that you are in the Python interpreter. To exit simply type 'exit\(\)' or 'ctrl+c / cmd+d'. Below you will find an example of this as well as an illustration of some useful methods. ![](/assets/interpreter.PNG)Returned from the help\(int\) call above within the Python interpreter:![](/assets/interpreterHelpMethod.PNG)

##### Functions

Functions are defined using the keyword 'def' and are called as you would call a function in many other languages. ![](/assets/pythonFunction.PNG)
