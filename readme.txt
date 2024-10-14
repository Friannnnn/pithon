

Python Data Structures – Maps
Python Maps also called ChainMap is a type of data structure to manage multiple dictionaries together as one unit. The combined dictionary contains the key and value pairs in a specific sequence eliminating any duplicate keys. The best use of ChainMap is to search through multiple dictionaries at a time and get the proper key-value pair mapping. We also see that these ChainMaps behave as stack data structure.


Creating a ChainMap
We create two dictionaries and club them using the ChainMap method from the collections library. Then, we print the keys and values of the result of the combination of the dictionaries. If there are duplicate keys, then only the value from the first key is preserved.


Creating a ChainMap

Creating a ChainMap

Map Reordering
If we change the order of the dictionaries while clubbing them in the above example, we see that, the position of the elements get interchanged as if, they are in a continuous chain. This again shows the behaviour of Maps as stacks.

Map Reordering

Map Reordering

Updating Map
When the element of the dictionary is updated, the result is instantly updated in the result of the ChainMap. In the below example, we see that the new updated value reflects in the result without explicitly applying the ChainMap method again.

Updating Map

Updating Map

Python Data Structures – Linked Lists
Lecture 6

Python Data Structures – Linked Lists

A linked list is a sequence of data elements, which are connected together via links. Each data element contains a connection to another data element in form of a pointer. Python does not have linked lists in its standard library. 

Python Data Structures – Linked Lists

We have already seen, how we create a node class and how to traverse the elements of a node. In this chapter, we are going to study the types of linked lists known as singly linked lists. In this type of data structure, there is only one link between any two data elements. We create such a list and create additional methods to insert, update and remove elements from the list.

Creation of Linked list
A linked list is created by using the node class we studied in the last chapter. We create a Node object and create another class to use this node object. We pass the appropriate values through the node object, to point them to the next data elements. The below program, creates the linked list with three data elements. In the next section, we will see how to traverse the linked list.

Creation of Linked list

Traversing a Linked List
Singly linked lists can be traversed in only forward direction starting from the first data element. We simply print the value of the next data element by assigning the pointer of the next node to the current data element.

Traversing a Linked List

Traversing a Linked List

Insertion in a Linked List
Inserting element in the linked list involves, reassigning the pointers from the existing nodes to the newly inserted node. Depending on whether the new data element is getting inserted at the beginning or at the middle or at the end of the linked list, we have the below scenarios.

Inserting at the Beginning
This involves pointing the next pointer of the new data node to the current head of the linked list. So, the current head of the linked list becomes the second data element and the new node becomes the head of the linked list.


Inserting at the Beginning



Inserting at the End
This involves pointing the next pointer of the the current last node of the linked list to the new data node. So the current last node of the linked list becomes the second last data node and the new node becomes the last node of the linked list.

Inserting at the End

Inserting at the End





Stacks
In the English dictionary, the word stack means arranging objects one over another. It is the same way; memory is allocated in this data structure. It stores the data elements in a similar fashion as a bunch of plates are stored one above another in the kitchen. So, stack data structure allows operations at one end, which can be called top of the stack. We can add elements or remove elements only form this end of the stack.


Python Data Structures - Dequeue
A double-ended queue, or deque, supports adding and removing elements from either end. The more commonly used stacks and queues are degenerate forms of deques, where the inputs and outputs are restricted to a single end.


Removing Element
In the example, we create a queue class, where we insert the data and then remove the data using the in-built pop method.
c

Adding Elements
In the example, we create a queue class,
where we implement the First-in-First-Out method. We use the
in-built insert method for adding data elements.


Python Data Structures - Queue
A queue can be implemented using python list, where we can use the insert() and pop() methods to add and remove elements.
There is no insertion as data elements are always added at the end of the queue.


Python Data Structures - Queue
We are familiar with queue in our day to day life as we wait for a service. The queue data structure also means the same, where the data elements are arranged in a queue. The uniqueness of queue lies in the way items are added and removed. The items are allowed at on end, but removed from the other end. So, it is a First-in-First out method.


Python Data Structures - Queue
We are familiar with queue in our day to day life as we wait for a service. The queue data structure also means the same, where the data elements are arranged in a queue. The uniqueness of queue lies in the way items are added and removed. The items are allowed at on end, but removed from the other end. So, it is a First-in-First out method.


POP from a Stack
As we know, we can remove only the top most data element from the stack, we implement a python program which does that. The remove function in the following program returns the top most element. We check the top element by calculating the size of the stack first and then, use the in-built pop() method to find out the top most element.


Stacks
In a stack the element inserted last in sequence, will come out first as we can remove only from the top of the stack. Such feature is known as Last in First Out(LIFO) feature. The operations of adding and removing the elements is known as PUSH and POP. In the following program, we implement it as add and remove functions. We declare an empty list and use the append() and pop() methods, to add and remove the data elements