
# Class 03

## Begin with a statement addressing why this topic matters as it relates to what you are studying in this module

* reading and writing files in Python is important as it allows us to manipulate and store data in external files. This can be useful for applications that require data persistence or for sharing data between different programs.

* Exception handling is also important in Python as it allows us to gracefully handle and recover from errors or unexpected events that may occur during program execution. By using try-except blocks, we can handle exceptions in a way that prevents our program from crashing or producing unexpected results. Overall, both file I/O and exception handling are important concepts to understand for any Python programmer.

## Reading  Questions

1. ### What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

* In Python, the 'with' statement is used to open and manage resources, such as files. It provides a convenient way of ensuring that the file is closed when the block of code inside the 'with' statement is exited, even if an exception is raised. This is important because forgetting to close a file can lead to resource leaks, and can cause errors when attempting to open the file again.

* When opening a file with the 'with' statement, you don't need to explicitly close the file as it will be done automatically. This helps to avoid common programming errors and ensures that resources are released as soon as they are no longer needed.

2. ### Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.

* 'read()' and 'readline()' are two different methods used to read files. The 'read()' method reads the entire content of a file and returns it as a single string. On the other hand, the 'readline()' method reads one line at a time and returns it as a string.

* To read the entire content of the file, we can use the 'read()' method
on the other hand, if we only want to read the first line of the file, we can use the 'readline()' method

3. ### Describe the concept of recursion in Python

* Exceptions are raised when an error or unexpected behavior occurs during program execution. Exception handling refers to the process of detecting and responding to these errors in a way that maintains the stability and correctness of the program.

* The ```try``` and ```except``` blocks are used to handle exceptions in Python. Code that might raise an exception is placed within the ```try``` block, and any exceptions that are raised are caught and handled within the ```except``` block. The ```finally``` block is used to specify code that should be executed regardless of whether an exception is raised or not, such as closing a file.

## Things I want to know more about

How to implement fault-tolerant servers
