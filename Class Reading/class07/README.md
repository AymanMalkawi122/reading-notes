
# Class 07

## Begin with a statement addressing why this topic matters as it relates to what you are studying in this module

* Big O notation helps us analyze the performance of algorithms, while local and global scopes help us organize our code and prevent naming conflicts.

## Reading  Questions

1. ### Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both?

    * Local scope refers to variables that are defined within a function and are only accessible within that function.

    * When a function is called, a new local scope is created, and any variables defined within the function are only accessible within that scope.

    * Global scope refers to variables that are defined outside of any function and are accessible throughout the entire program.

    ```python
        sum = 0 # global

        def my_function(arr):
            for ele in arr:
                sum += ele
        arr = [1, 2, 3]        
        my_function(arr)

        print(x)
    ```

2. ### How do the global and nonlocal keywords work in Python, and in what situations might you use them?

    * variables can have either global or local scope. The global keyword is used to declare a variable outside of a function, whereas the nonlocal keyword is used to declare a variable in an enclosing function.

    * When a variable is declared as global, it can be accessed and modified from any part of the code, including inside functions. However, if a variable is declared inside a function, it is considered to have local scope and can only be accessed from within that function, unless explicitly declared as global or nonlocal.

    * Global is used to access and modify global variables from within a function, while nonlocal is used to access and modify variables from the nearest enclosing scope that is not global.

3. ### In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis?

    * The purpose of Big O notation is to analyze the efficiency of algorithms and to identify bottlenecks in the algorithm's performance.

4. ### explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials?

    * To simulate a dice roll, we can use the random module which has a function called ```randint().``` which returns a random integer between the specified range.

    * To calculate the probability of rolling a specific number we can do roll of a dice multiple times and count the number of times the specific number is rolled then devide it by the total amount of rolls and it should approximate to 1/6.

## Things I want to know more about

How to improve your Big O analytical skills.
