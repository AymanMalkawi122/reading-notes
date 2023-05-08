
# Class 04
## Begin with a statement addressing why this topic matters as it relates to what you are studying in this module.

* Classes and Objects are important for creating reusable and modular code, Pytest Fixtures are important for setting up consistent test environments, and Coverage is important for ensuring comprehensive testing of your code.

## Reading  Questions

1. ### What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?

* A class is a blueprint or template for creating objects, while an object is an instance of a class.

* Classes define the attributes and behaviors of objects, while objects are instances of classes that have specific values for their attributes.

2. ### Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?

* Recursion is a programming technique where a function calls itself until a condition is met. In Python, recursion can be used to solve problems that can be broken down into smaller sub-problems.

* Here's an example of how recursion can be used to calculate the Fibonacci sequence:
```
def fib(n):
    if n <= 0:
        return 0
    if n == 1
        return 1

        return fib(n - 1) + fib(n - 2)
```

3. ### What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project.

* Pytest fixtures are a way to set up a pre-determined state for a test or a set of tests. by using fixtures, we can avoid repeating the same setup code in multiple tests, which can help to make our tests more readable and maintainable.

* Code coverage, is a measure of how much of our code is actually being executed during testing. By measuring code coverage, we can identify parts of our code that are not being tested, and we can make sure that our tests are enough to cover all of our code.

## Things I want to know more about
How to identify crucial code blocks  that require intensive testing