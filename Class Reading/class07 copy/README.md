
# Class 08

## Begin with a statement addressing why this topic matters as it relates to what you are studying in this module

* Decorators are widely used in Python for various purposes, such as logging, input validation, authentication, caching, and more.

* They provide a powerful and flexible way to modify the behavior of functions or classes without modifying their original code, promoting code reusability and separation of concerns.

## Reading  Questions

### 1. What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers?

    * The basic syntax of Python list comprehension allows us to create a new list by applying an expression to each element of an existing iterable, such as a list, and optionally filtering the elements based on a condition.

    * List comprehension provides a concise and readable way to create lists compared to using traditional for loops.

### Example

```python
    #using comprehension
    numbers = [1, 2, 3, 4, 5]
    by_two_numbers = [num * 2 for num in numbers]
    #numbers = [2, 4, 6, 8, 10]
```

```python
#using for loop
numbers = [1, 2, 3, 4, 5]
by_two_numbers = []
for num in numbers:
    by_two_numbers.append(num * 2)
#numbers = [2, 4, 6, 8, 10]
```

### 2. What is a decorator in Python?

* a decorator is a function that takes another function as input and extends or enhances its functionality.
* It allows us to add extra features, modify the behavior, or perform some actions before and after the execution of the decorated function.

### 3. Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading?

* decorators are a way to modify the behavior of functions or classes without changing their source code.
* They allow you to wrap or decorate a function or class with additional functionality.

1. **Logging**: Decorators can be used to add logging statements before and after function execution to track its behavior or performance.
2. **Timing**: Decorators can measure the time taken by a function to execute and provide performance insights.
3. **Authentication**: Decorators can enforce authentication checks before allowing access to certain functions or methods.

### Example

```python
    def validate_inputs(func):
    def wrapper(*args, **kwargs):
        for arg in args:
            if not isinstance(arg, int):
                raise ValueError("Invalid input! Only integers are allowed.")
        return func(*args, **kwargs)
    return wrapper

@validate_inputs
def multiply_numbers(a, b):
    return a * b

result = multiply_numbers(5, 10)
print(result)

result = multiply_numbers(5, "hello")
print(result)
```

## Things I want to know more about

How to improve my code reusabilty
