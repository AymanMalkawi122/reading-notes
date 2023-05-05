
# Data Structures and Algorithms
## Begin with a statement addressing why this topic matters as it relates to what you are studying in this module.
This topic is extremely important because choosing the right data structure can boost the performance of our application dramatically. 

Performance can be measured by how much resources the application takes up, like time and space but after advances in hardware technology, time usually has more priority over space.

## Discussion Questions

1. What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?

How read and write operations will be done on the data structure, for example, if I have five users and I want to store their data I could use a list of lists that will perform like this.

* ADD: O(1) because we can add a new user to the end of the list and that's it
* DELETE, UPDATE, and READ: O(n) because these operations by themselves are not the reason for the O(n) complexity but the reason is that we have to find the user in the list before we can perform any operation.

On the other hand, if we use a hash map to store our lists the performance will go as follows.

* ADD: O(1) because we can add a new user to the hash map instantly in an ideal collision-free environment.
* DELETE, UPDATE, and READ: O(1) because we can find the user in the hash map instantly in an ideal collision-free environment.

We can't have an ideal collision-free hash map but we can come close to it by increasing the hash map's capacity based on how much data we store in it so we can have a low collision percentage.

this does not mean that a hash is a solution for every problem, it just means that for this specific scenario, a hash map is better than a list.

2. How can we ensure that we’ll avoid an infinite recursive call stack?

By making sure that our recursive function will always converge to our base case, then our base case will terminate the recursive behavior of our function
## Things I want to know more about
How we can use and maintain data structures like a Binary Tree or a Heap because, for example if we don't balance the binary tree, it will lose a lot in performance or if we don't heapify our Heap after each pop operation it will lose its key feature, which is storing the least or the highest value in the root.
