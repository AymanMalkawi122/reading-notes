
# Class 02

## Begin with a statement addressing why this topic matters as it relates to what you are studying in this module

TDD helps ensure the correctness and functionality of our code, while packages and modules help us organize, modularize, and reuse our code efficiently, which helps us to adhere to the single responsibility rule.

## Reading  Questions

1. ### What are the key principles of Test-Driven Development (TDD) in Python, and how do they contribute to the overall quality of code?

* TDD is a way of writing code that emphasizes testing our code before we even start writing it. by writing a test that our code needs to pass, and then we write the code that passes that test.

2. ### Explain the purpose of the if __name__ == '__main__': statement in Python scripts. What are some use cases for including this conditional in your code?

* The if __name__ == '__main__'  is used to control the behavior of a script when it's executed, it allows us to specify which code block will run when the script is run as the main program.

* A use case for this statement is when a Python module can be a standalone script or imported into another script, for example, if run a module that sums an array of numbers as the main function it should print the result instead of returning it.

3. ### Describe the concept of recursion in Python

* Recursion is a method where a function calls itself like a loop, but instead of the loop condition reaching a False state, it calls itself until it reaches a base case.

* The base case is the condition that stops the recursive function and prevents an infinite loop.

4. ### What is the difference between Python modules and packages? Explain how to create, import, and use them in your Python programs

* Python modules are single files that contain Python code, while Python packages are collections of modules and internal packages.

* To create a Python module, we can simply write our code in a file with the .py extension and save it in any directory.

* To create a package, we create a directory with an init.py file and add any number of modules or sub-packages to it.

* To import a module or package in a Python program, we can use the import statement followed by the name of the module or package.

## Things I want to know more about

I want to go more in-depth on Test-Driven Development.
