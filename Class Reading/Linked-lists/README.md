# Linked Lists

Linked lists are used in programming because they provide a flexible and efficient way to store and manipulate data. They consist of a sequence of nodes, each containing a value and a reference to the next node in the list. To add or delete nodes, you update the references of the surrounding nodes. Traversing a linked list involves following the references from the head node until the end of the list is reached.

## Use WHY, WHAT, HOW structure

1. **WHY** are linked lists used in programming? Linked lists are used in programming because they provide a flexible and efficient way to store and manipulate data. Unlike arrays, which have a fixed size, linked lists can grow or shrink dynamically as needed.

    Linked lists are also useful when the order of data is important, as they allow for easy insertion or deletion of elements anywhere in the list.

2. **WHAT**

    What is a linked list? A linked list is a data structure consisting of a sequence of nodes, where each node contains a value and a reference to the next node in the list.

    The first node is called the head, and the last node is called the tail. The tail node has a reference to NULL, which indicates the end of the list.

3. **HOW**

    How do linked lists work? To add a new node to a linked list, you first allocate memory for the new node and assign its value. Then, you update the reference of the previous node to point to the new node, and update the reference of the new node to point to the next node.

    To delete a node, you update the reference of the previous node to point to the next node, and deallocate the memory used by the deleted node.

    Traversing a linked list involves iterating through the list from the head node, following the reference to the next node until the end of the list is reached.
