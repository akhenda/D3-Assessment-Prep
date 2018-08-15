## Output:

Make a list of _at minimum_ five data structures you might use in your work, and map them to examples of when they would be used.

#### Arrays

> An array is an ordered collection of items, where each item inside the array has an index.

We use them a lot in our day to day work e.g. an array of middlewares to be dispatched to redux `applymiddleware` function during store configuration.

#### Stacks

> Just like the arrays and lists, stacks and queues are also collection of items. They are just different ways we can hold multiple items. It’s last in, first out data structure, with no care about numeric indexes.

One of the best uses for a stack in programming is when parsing code or expressions, where you need to do something like validating the correct amount of opening and closing curly braces, square brackets or parenthesis.

Stacks are also used in forward/backward feature in web browsers and undo/redo operations in text editors and word processors.

In interview questions, they can be used to find the correct path in a maze using backtracking.

Typical application areas include compilers, operating systems, handling of program memory (nested function calls)

#### Queues

> The key difference between a stack and a queue. Stacks are last in first out (LIFO), while queues are first in first out (FIFO). And as with stacks, we should not even be thinking about numeric indexes.

Queues are very commonly used in concurrency situations to keep track of what tasks are waiting to be performed and making sure we take them in that order i.e. when a resource is shared among multiple consumers like in CPU scheduling, Disk Scheduling.

Typical application areas include print job scheduling, operating systems (process scheduling).

#### Priority Queues

> Some languages offer a version of a queue, called a priority queue. This allows you to arrange elements in the queue based on their priority.

It’s a queue, where items with higher priority step ahead of items with lower priority in the queue.

They are used in process scheduling in the kernel.

#### Hash Table

> It’s a typical data structure to implement an associative arrays; mapping keys to values.
>
> It's a dictionary-like data structure which pairs keys to values.

It is used for fast data lookup - symbol table for compilers, database indexing, caches, unique data representation.

Inspired by the Internet, **blockchain** technologies seek to open source the very structure of the web. By using hash functions to create immutable fingerprints for every block of data, essentially the entire database can exist openly on the web for anyone to see and contribute to.


#### Binary Search Tree

> This is a binary tree where the value of each node is greater than or equal to the value of left subtree & the value of each node is less than or equal to the value of right subtree.

It is used to implement multilevel indexing in database. It is also used in Huffman Coding Algorithm & to implement searching Algorithm.

Used in many search applications where data is constantly entering/leaving, such as the `map` and `set` objects in many languages' libraries such as JavaScript's `immutable` library.

#### Heap

> It is a specialised tree data structure that satisfies the following property: if P is a parent node of C, then the value of P is either greater than or equal to (in a max heap) or less than or equal to (in a min heap) the value of C.
>
> Heaps are usually implemented using the idea of a binary tree, not a binary search tree but still, a binary tree. They’re a way of implementing other abstract data types like the priority queue.

Heap is used in Heapsort & in Dynamic memory allocation in lisp.

#### Graph

> This is a data structure that consists a finite set of vertices called as Nodes & a finite set of ordered pair called as Edge. Graph can be Directed or Undirected.

Graphs are used to represent networks. Graphs are also used in social networks like linkedIn, facebook. For example, in facebook, each person is represented with a vertex(or node). Each node is a structure and contains information like person id, name, gender and locale. They are also used in _Routing Algorithms_ e.g. **OSPF** (Open Shortest Path First), **RIP** (Routing Information Protocol) and **BGP** (Border Gateway Protocol)

#### Reference

-   [StackOverflow](https://stackoverflow.com/questions/1539069/practical-uses-of-different-data-structures)
-   [Quora](https://www.quora.com/What-are-the-applications-of-data-structures)

#### NB: Difference between an Abstract Data Type(ADT) and a Data Structure

To put it simple, ADT is a logical description and data structure is concrete. ADT is the logical picture of the data and the operations to manipulate the component elements of the data. Data structure is the actual representation of the data during the implementation and the algorithms to manipulate the data elements. ADT is in the logical level and data structure is in the implementation level.

[ADT vs DS](https://abrickshort.wordpress.com/2005/03/06/abstract-data-types-vs-data-structures/)

-----

## Knowledge

**1.  How to determine the best data structure for an end goal**

Data structure is a particular way of organizing data in a computer. The developer must choose the appropriate data structure for better performance i.e. time and space considerations. If the developer chooses bad data structure, the system does not perform well.

Also, operations such as `access`, `insert`, `delete`, `find`, & `sort` dictate the type of data structure to use.

**2.  Benefits and drawbacks of the most common data structures**

| Data Structure 	| Advantages                                                      	| Disadvantages                                                                	|
|----------------	|-----------------------------------------------------------------	|------------------------------------------------------------------------------	|
| **Array**          	| Quick insertion. Very fast access if the index is known. It can be used to implement other data structures like linked lists, stacks, queues, trees, graphs etc.	| Slow search. Slow deletion. Fixed size. Array is static structure. It means that array is of fixed size. The memory which is allocated to array can not be increased or reduced. Since array is of fixed size, if we allocate more memory than requirement then the memory space will be wasted. And if we allocate less memory than requirement, then it will create problem.	|
| **Ordered Array**  	| Quicker search than unsorted array                              	| Slow insertion and deletion. Fixed size.                                     	|
| **Stack**          	| Provides last-in, first-out access.                             	| Slow access to other items.                                                  	|
| **Queue**          	| Provides first-in, first-out access.                            	| Slow access to other items.                                                  	|
| **Linked List**    	| Quick insertion. Quick deletion.                                	| Slow search.                                                                 	|
| **Binary Tree**    	| Quick search, insertion, deletion (if tree remains balanced).   	| Deletion algorithm is complex.                                               	|
| **Red-Black Tree** 	| Quick search, insertion, deletion. The Tree is always balanced. 	| Complex.                                                                     	|
| **Hash Table**     	| Very fast access if the key is known. Fast insertion            	| Slow deletion. Access is slow if key is not known. Inefficient memory usage. 	|
| **Heap**           	| Fast insertion, deletion, access to largest item.               	| Slow access to other items.                                                  	|
| **Graph**          	| Models real-world situations.                                   	| Some algorithms are slow and complex.                                        	|

**3.  How each data structure actually works in computer memory**

-   [Data Structures](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/data-structures)

**4.  How to communicate in “Big-O” notation (refresher)**

This is a theoretical measure of the execution of an algorithm, usually the time or memory needed, given the problem size **n**, which is usually the number of items. Informally, saying some equation `f(n) = O(g(n))` means it is less than some constant multiple of `g(n)`.

It is used in Computer Science to describe the performance or complexity of an algorithm. Big-O specifically describes the worst-case scenario, and can be used to describe the execution time required or the space used (e.g. in memory or on disk) by an algorithm.

The most optimum algorithm scales in _constant_ time and space. This means it does not care at all about the growth of its inputs. Next best is _logarithmic_ time or space, then _linear_, _linearithmic_, _quadratic_, and _exponential_. The worst is _factorial_ time or space. In **Big-O** notation:

-   **Constant:** O(1)
-   **Logarithmic:** O(log n)
-   **Linear:** O(n)
-   **Linearithmic:** O(n log n)
-   **Quadratic:** O(n²)
-   **Expontential:** O(2^n)
-   **Factorial:** O(n!)

**5.  How and when to use Binomial & Fibonacci heaps**

###### Binomial Heaps
A simple, flexible, and versatile priority queue.

A **priority queue** is a data structure that stores a set of elements annotated with keys and allows efficient extraction of the element with the least key. Priority queues are frequently implemented as **binary heaps**. A **binary heap** is a binary tree **(NOT a BST)** that is:

-   **Complete**: the tree is completely filled except possibly the bottom level, which is filled from left to right
-   **Satisfies the heap order property**
    -   every node is less than or equal to its children
    -   or every node is greater than or equal to its children

The root node is always the smallest node or the largest, depending on the heap order.

A **binomial tree** of **order k** is a type of tree recursively defined as follows:
> A binomial tree of order k is a single node whose children are binomial trees of order 0, 1, 2, …, k – 1.

A heap-ordered binomial tree is a binomial tree whose nodes obey the heap property: all nodes are less than or equal to their descendants.

Therefore, a **binomial heap** is a collection of heap-ordered binomial trees stored in ascending order of size.

Binomial heaps use a singly linked circular link list for linking the nodes.

###### Fibonacci heaps

Fibonacci heaps differ from binomial-heaps, however, in that they have more more relaxed structure allowing for improved asymptotic time bounds work that maintains the structure is delayed until it is convenient to perform.

Like a binomial heap, a fibonacci heap is a collection of heap-ordered trees however, trees are not constrained to be binomial trees.

Trees within fibonacci heaps are rooted but unordered.

The roots of all trees are also linked together using their left & right pointers into a **circular, doubly-linked list** which is called the root list. Circular, doubly-linked lists have two advantages for use in **fib-heaps**:
-   we can remove a node in O(1) time
-   given two such lists, we can concatenate them in O(1) time.

###### Differences
-   Binomial heap takes O(log n) time in all operations while Fibonacci heap takes amortized running time O(1) in Insert, find, decrease key operations and O(log n) time in delete min, delete operations.
-   Binomial heaps use a singly linked circular link list and Fibonacci heaps use a doubly linked circular linked list.
-   Every Binomial heap is a Fibonacci heap but every Fibonacci heap isn't Binomial heap.
-   Delete-min in Binomial heaps involves the combining of trees where as delete-min or delete in Fibonacci heaps is performed without joining the trees obtained after deletion.
-   Data members in a node for Binomial heaps are data, link, degree and child. Whereas in Fibonacci heaps it is data, parent, childcut, child, link and degree.

###### Applications
-   Binary heaps are used in the priority queues. Priority queues are widely used in the real systems. One known example is **process scheduling** in the kernel. The highest priority process is taken first.
-   Fibonacci heap is used to improve the asymptotic running time of Dijkstra's algorithm (single-source shortest path), Prim's algorithm (minimum spanning tree) or Huffman encoding (data compression).

**6.  How and when to use AVL/Red black trees**

###### AVL Tree

Named after their inventor **Adelson**, **Velski** & **Landis**, **AVL trees** are height balancing binary search tree. AVL tree checks the height of the left and the right sub-trees and assures that the difference is not more than 1. This difference is called the **Balance Factor**.

In computer science, an AVL tree is a self-balancing binary search tree, and it is the first such data structure to be invented.

When to use AVL Tree?

It is observed that BST's worst-case performance is closest to linear search algorithms, that is Ο(n). In real-time data, we cannot predict data pattern and their frequencies. So, a need arises to balance out the existing BST.

To balance itself, an AVL tree may perform the following four kinds of rotations; `left`, `right`, `left-right` and `right-left` rotations.

AVL tree structures can be used in situations which require fast searching. But, the large cost of re balancing may limit the usefulness.

AVL trees are applied in th e following situations:

-   There are few insertion and deletion operations
-   Short search time is needed
-   Input data is sorted or nearl y sorted

Databases are just one application of AVL Trees. With the advent of **solid state drives**, AVL Trees will take over the database market and render B+ Trees obselete.

###### Red-Black Trees

Red - Black Tree is another self-balancing variant of Binary Search Tree in which every node is colored either **RED** or **BLACK**.

In a Red Black Tree the color of a node is decided based on the following Red Black Tree properties.

-   Red - Black Tree must be a Binary Search Tree.
-   The ROOT node must colored BLACK.
-   The children of Red colored node must colored BLAC-   (There should not be two consecutive RED nodes).
-   In all the paths of the tree there must be same number of BLACK colored nodes.
-   Every new node must inserted with RED color.
-   Every leaf (e.i. NULL node) must colored BLACK.

In AVL tree insertion, we used rotation as a tool to do balancing after insertion caused imbalance. In Red-Black tree, we use two tools to do balancing, **Recoloring** and **Rotation**. We try recoloring first, if recoloring doesn’t work, then we go for rotation.

Red-black tree is a kind of balanced tree (others are AVL-trees and 2-3-trees) and can be used everywhere where trees are used, usually for the fast element searches. E.g., it is used in some implementations of C++ STL (Standard Template Library) for sets and maps.

K-mean Clustering using red black tree, Databases, searching words inside dictionaries, searching on web.

**7.  How and when to use Splay Trees**

Splay tree is another variant of binary search tree. In a splay tree, the recently accessed element is placed at the root of the tree.

Splay Tree is a self - adjusted Binary Search Tree in which every operation on an element rearranges the tree so that the element is placed at the root position of the tree.

In a splay tree, every operation is performed at root of the tree. All the operations on a splay tree are involved with a common operation called "Splaying".

Splaying an element is the process of bringing it to the root position by performing suitable rotation operations.

In a splay tree, splaying an element rearranges all the elements in the tree so that splayed element is placed at root of the tree.

###### Applications of Splay trees
-   Due to their reference of locality property, they can be used in implementing logic behind caches.
-   They can come handy in joining two trees – merging a tree between 2 elements of another tree (O(log M + N))
-   Also they can be used in bifurcating the data into 2 distinguish data sets – cutting a tree
-   Can be used in garbage collectors
-   Querying faster than O(log(N)) for highly biased query distributions
-   Used in network router

**8.  How and when to use Skip Lists**

Skip lists are a linked-list-like structure which allows for fast search. It consists of a base list holding the elements, together with a tower of lists maintaining a linked hierarchy of subsequences, each skipping over fewer elements.

###### Applications

Can be used as a replacement for BST. The main advantage of using Skiplists over BST is that it is best suited for concurrent access.

**9.  How and when to use tries**

A trie is a `tree-like` data structure whose nodes store the letters of an alphabet. By structuring the nodes in a particular way, words and strings can be retrieved from the structure by traversing down a branch path of the tree.

**Trie** is an efficient information re**Trie**val data structure. Using Trie, search complexities can be brought to optimal limit (key length).

###### Applications
There are many cool applications of tries. Autocomplete on text inputs. This maybe the most common application of the trie. Once you've typed in a letter, the tree of potential words is greatly reduced, allowing the program to easily enumerate what kinds of strings are possible.

If all you wanted to do was to store words, a state machine might be easier. However, the trie can store additional information for each word. For example, the trie can store how popular a word might be. That's why when you type "ye", "yes" is suggested before "yelling".

Tries are also useful for approximate matching algorithms, like those used in spell check. A slightly misspelled word will have a similar path from the root of the tree when compared with the correctly spelled word. This is especially true if certain modifications are made to the trie, like branch merging.

String matching is another use case where tries and approximation algorithms are useful. Longest suffix or prefix matching uses these methods.

Tries can also be used for sorting. Using a trie to do this is similar to radix sort. A pre-order traversal of the tree will result in an output that is in increasing order, allowing sorting.
