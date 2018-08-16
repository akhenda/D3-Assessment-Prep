## Output:

Make a list of *at minimum* five algorithm types you might use in your work, and map them to examples of when they would be used.

#### Math Algorithms

-   [Factorial](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/math/factorial)
-   [Fibonacci](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/math/fibonacci)

#### Searching Algorithms

-   [Linear Search](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/searching/linear-search)
-   [Binary Search](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/searching/binary-search)

#### Sorting Algorithms

-   [Shell Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/tree/develop/src/algorithms/sorting/shell-sort)
-   [Quick Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/sorting/quick-sort)
-   [Merge Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/sorting/merge-sort)
-   [Bubble Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/sorting/bubble-sort)
-   [Insertion Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/sorting/insertion-sort)
-   [Selection Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/sorting/selection-sort)

-----

## Knowledge

**1.  How and when to use search algorithms**

Although developers can choose from numerous search types, we select the algorithm that best matches the size and structure of the database to provide a user-friendly experience.

The general searching problem can be described as follows: Locate an element `x` in a list of distinct elements `a1,a2,...aN` or determine that it is not in the list. The solution to this search problem is the location of the term in the list that equals `x` and is 0 if `x` is not in the list.

**2.  How and when to use `greedy algorithms`**

Greedy algorithms choose the best option at the current time, without any consideration for the future.

Greed is not always good- you may end up with a non-optimal solution (using more fuel than you could have). This is the natural trade-off for being a short-term visionary rather than a long-term visionary.

Let us see an elementary example where it fails. See the following directed network:

![Greed si poa manze](https://i.imgur.com/WoWY9F9.png)

Going by the intuition, you would choose first A and then you are stuck with the road of length 99. So you end up moving 100 units rather than a possible 10- had you visited B first, which did not seem attractive then. So greedy algorithm fails in this case. So why even use it? Because many times it works giving optimal solution while simply applying layman instincts. It turns out this network does have a greedy optimal solution but there computations must be done before leaving- in an intelligent manner. It is called **Djikstra’s algorithm**. This network is too simplistic to feel the algorithm, and is best used for counterexamples. It’ll need a complex network to appreciate this algorithm.

When the greedy method doesn’t work, we look forward to something called **dynamic programming** methods.

**3.  How and when to use divide-and-conquer programming**

This paradigm, **divide-and-conquer**, breaks a problem into subproblems that are similar to the original problem, recursively solves the subproblems, and finally combines the solutions to the subproblems to solve the original problem. Because **divide-and-conquer** solves subproblems recursively, each subproblem must be smaller than the original problem, and there must be a base case for subproblems. You should think of a **divide-and-conquer** algorithm as having three parts:

1.  **Divide** the problem into a number of subproblems that are smaller instances of the same problem.
2.  **Conquer** the subproblems by solving them recursively. If they are small enough, solve the subproblems as base cases.
3.  **Combine** the solutions to the subproblems into the solution for the original problem.

You can easily remember the steps of a divide-and-conquer algorithm as _divide_, _conquer_, _combine_.

Usually this method can be used when the problem at hand, can be reduced to solving non-overlapping sub-problems and combining the result, and also there should be a base case in which the solution to the problem is trivial.

A problem can be solved using divide and conquer when the given problem can be :

1.  Divided into a number of subproblems that are smaller instances of the same problem.
2.  Each subproblem can be solved recursively which basically means each instance of the subproblem is identical in nature.
3.  The solutions of each subproblem can be combined so as to solve the problem at hand.

Some algorithms that use this method:

-   Quick Sort
-   Merge Sort
-   Binary Search
-   Tower of Hanoi
-   Pascal's Triangle
-   Euclidean Algorithm - GCD
-   Tree Depth-First Search (DFS)
-   Graph Depth-First Search (DFS)
-   Permutations (with and without repetitions)
-   Combinations (with and without repetitions)
-   Maximum sub-array problem
-   Strassen’s algorithm for matrix multiplication

**4.  How and when to use dynamic programming/dynamic optimization**

Dynamic Programming (DP) is used to solve an optimization problem by caching subproblem solutions (memoization) rather than recomputing them.

Dynamic Programming algorithms are often used for optimization because they will examine the previously solved subproblems and will combine their solutions to give the best solution for the given problem.

Now, problems that can be solved by a Dynamic Programming Algorithm will have this necessary condition:

> **Principle of Optimality**: An optimal policy has the property that whatever the initial state and initial decision are, the remaining decisions must constitute an optimal policy with regard to the state resulting from the first decision.

**5.  How and when to use reactive programming**

Simply put, **Reactive Programming** is programming with asynchronous data streams.

To give an example, in Javascript you have **promises** and **callbacks**. A promise/callback could be thought of as data streams that emit one event (the event which represents the completion of the previous function).

Reactive Programming is the process of setting up these data flows and linking their events to actions in the system.

###### Why Should We Use It?
1.  **Reactive Code is easier to reason about** - Reactive code allows us to focus on interdependent events. This makes separation of concerns easier than reasoning about implementation details in a large system.
2.  **We avoid "Callback Hell"** - Events abstract away the need for explicit callbacks and the awful amount of nesting that comes with them. The result is cleaner, more readable code.
3.  **Models interactive apps nicely** - Modern apps are highly interactive. There's live feeds, ajax calls when buttons are clicked, synchronization of state between multiple clients. Data streams capture this functionality really nicely without having to build out your own massaging systems from scratch.
4.  **Better Usage Of Resources** - Since all our code is asynchronous, multiple tasks can be accomplished at the same time. This better utilizes our computers resources and makes our applications run faster.

###### Where Should We Use It?
It's a tool like anything else and we should apply it where it fits. Knowing where to apply it may be hard at first, but as it becomes more familiar, we gain a better intuition on how to use it.

###### Reference
-   [Quora (I love this site. It has very sober minds.)](https://www.quora.com/What-is-reactive-programming-Why-should-we-use-it-and-where)

**6.  How and when to use graph algorithms**

Graphs are applied widely nowadays. They are used in economy, aeronautics, physics, biology (for analyzing DNA), mathematics and other areas.

Below are some examples where Graph Algorithms are used.

###### Shortest Path:

This is probably the most often used algorithm. It may be applied in situations where the shortest path between 2 points is needed.

Examples of such applications would be:

-   **Computer games** - finding the best/shortest route from one point to another.
-   **Maps** - finding the shortest/cheapest path for a car from one city to another, by using given roads.
-   May be used to find the fastest way for a car to get from one point to another inside a certain city. E.g. satellite navigation system that shows to drivers which way they should better go.

###### Minimal Spanning Tree:

-   Consider some communications stations (for telephony, cable television, Internet etc.) and a list of possible connections between them, having different costs. Find the cheapest way to connect these stations in a network, so that a station is connected to any other (directly, or through intermediate stations). This may be used for example to connect villages to cable television, or to Internet.
-   The same problem, but instead of connecting communications stations - villages are to be connected with roads.

###### Eulerian Path/Circuit:

A postman has to visit a set of streets in order to deliver mails and packages. It is needed to find a path that starts and ends at the post-office, and that passes through each street (edge) exactly once. This way the postman will deliver mails and packages to all streets he has to, and in the same time will spend minimum efforts/time for the road.

###### Network Flows:
With Maximum Flow algorithm it is possible to find the most loaded roads or rails in a certain transportation network, and also to determine its maximum intensivity. This information may be then used to improve the traffic situation in those places.
Optimal Graph Coloring:
This algorithm may be used to color a map with a minimum number of colors.

###### Graph Median:

A warehouse should be placed in a city (a region) so that the sum of shortest distances to all other points (regions) is minimal. This is useful for lowering the cost of transporting goods from a warehouase to clients.
Same thing can be considered for selecting the place of a shop, market, office and other buildings.

###### Graph Center:

Suppose that a hospital, a fire department, or a police department, should be placed in a city so that the farthest point is as close as possible. For example a hospital should be placed in such a way that an ambulance can get as a fast as possible to the farthest situated house (point).

**7.  How to identify and work with NP problems**

A problem is NP if it is easy to verify a solution. It might not be easy to find such a solution, but given a candidate solution, we can easily verify whether it is in fact a solution or not.

For example, consider the Travelling Salesperson Problem. We have a graph representing cities and roads. The salesperson needs to find a route traversing all cities exactly once, which is as short as possible. Let’s say they need to find a route shorter than some threshold x. Given a candidate solution, we just add up all the distances and check whether or not this is shorter than x. Easy enough, and the time it takes will be roughly linear in the number of cities.

However, finding whether such a solution exists or not is far from trivial; in fact, it is known to be NP-complete (if we find an efficient solution, which takes time polynomial in the number of cities, we can find such a solution to any NP problem).

--

Proving something is in NP is usually fairly easy. You imagine that some Oracle gives you a solution to the problem. Then you see if there is a way to check that the solution is correct using only polynomial time algorithms.

For example, consider the problem of “What is the smallest number in this list?” You imagine that the Oracle tells you, “The smallest number is 4”. You loop through the list, looking for numbers less than 4, and you won’t find any. You will now know that the smallest number is indeed 4. It took you only O(n) steps, a polynomial time algorithm.

Of course, that was too easy, since that problem is in P. Its not hard to find a polynomial time algorithm even without the Oracle. But there are other cases where there doesn’t seem to be a polynomial time algorithm for finding it, even though there is one for checking it. A famous example is 3SAT, where you’re looking for assignments of variables (a=true, b=true, c=false, d=true, etc) and you want to see if some set of statements (a AND b AND NOT c; NOT a AND NOT D) are all true. Easy to check a proposed solution, but it looks like there’s no better way to find a solution than to try all of the possiblities, which takes O(2n) time.

That problem and many others are in NP but not (apparently) in P. In particular, that one is NP-complete: if you can solve it in some time, you can solve ALL NP problems in that time.

Proving a problem is NP-complete is a lot more effort: you usually have to prove it’s equivalent to some other known NP-complete problem.

The real question is whether there are NP-complete problems that aren’t in P. That’s a whole ‘nother kettle of fish.

###### Reference

-   [Quora](https://www.quora.com/How-do-I-determine-if-an-algorithm-is-NP-or-not)

**8.  How to determine the appropriate algorithm for a goal**

We do this by determining the amount of resources (such as time and storage) necessary to execute them. Usually, the efficiency or running time of an algorithm is stated as a function relating the input length to the number of steps (time complexity) or storage locations (space complexity).

In theoretical analysis of algorithms it is common to estimate their complexity in the asymptotic sense, i.e., to estimate the complexity function for arbitrarily large input. Big O notation, Big-omega notation and Big-theta notation are used to this end. For instance, binary search is said to run in a number of steps proportional to the logarithm of the length of the sorted list being searched, or in O(log(n)), colloquially "in logarithmic time". Usually asymptotic estimates are used because different implementations of the same algorithm may differ in efficiency. However the efficiencies of any two "reasonable" implementations of a given algorithm are related by a constant multiplicative factor called a hidden constant.

Complexity is measured (informally), using [Big-O Notation](https://github.com/akhenda/es6-data-structures-and-algorithms#big-o-notation), and is written as O(x), where x is some mathematical expression that relates to the number of inputs (commonly called n inputs).

So, for example,

-   An O(1) program completes in the same amount of time, regardless of its inputs.
-   An O(n) program completes in an amount of time that is in direct proportion with its inputs.
-   A O(n2) algorithm completes in the square of n (n time n).

**9.  How to work with various sorting data sets, such as:**

-   [Shell Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/tree/develop/src/algorithms/sorting/shell-sort)
-   [Quick Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/sorting/quick-sort)
-   [Merge Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/sorting/merge-sort)
-   [Bubble Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/sorting/bubble-sort)
-   [Insertion Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/sorting/insertion-sort)
-   [Selection Sort](https://github.com/akhenda/es6-data-structures-and-algorithms/blob/develop/src/algorithms/sorting/selection-sort)

**10.  Definition of hash algorithms and the problems they aim to solve**

Hashing algorithms are widely used in computer security.

With the advent of distributed computing in modern internet applications, they have become increasingly important. Whether it is associating machines with incoming requests or horizontally distributing data to particular machines, the use of hashing algorithms might be internal but very pervasive. All languages use some sort of hashing algorithms for storing key/value pairs in map or hashtables.

In any use case, where you need to identify a value based on some sort of key, system will inadvertently fall back on hashing. Understanding the concept behind hashing algorithm has certainly helped me in multiple ways. I have come to appreciate the concept of prime numbers, have learned quite a lot about bit operators & idea behind key spaces and associated overflows etc.

One use of hashing algorithms worth mentioning is Protecting Identity (making data anonymous)

A simple use of hash function(hashing) converts the username/user id to a hashID to protect identity and still making sure John points to hash(John).

e.g.: always john_id will convert with same hash function to something like `abcd1234efghi678`

```python
diffcult_to_reverse_hash_function(john_id) = 'abcd1234efghi678'
```

This `abcd1234efghi678` now represents John in a given system and "protects" his identity from being revealed/identified by a person/analyst.

Hash functions are difficult to reverse. But its not impossible to find an inverse of hash function as crypto folks say.

Hashing has following uses:
1. In Hash Tables
2. To build caches
3. In cryptography
4. In Rabin-Karp algorithm to search substrings
5. In computer graphics etc.

Also, the difficulty in deriving the key from the hash makes hashing useful in crypto-currencies where transactions are logged by the concept of Proof-of-work system. Bitcoin is an example. It uses two  `SHA-256` back-to-back.

There are a lot of different hashing algorithms. Some cryptographic hashing algorithms are `MD5`, `SHA1`, `SHA256`, `SHA384` and `SHA512`.
