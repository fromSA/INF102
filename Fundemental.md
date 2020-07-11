# Fundementals
- Algorithms go hand in hand with data structures
- ADT (abstract data types) for modular programming
- API (Applications programming interface)

***'Algorithm'*** Noun 

finite, determinstic and effective problem-solving method suitable for implementation as a computer program.

A computer program is just one way of express an algorithm



## Analysis of algorithms
Time
Space

## Algorithms: 
### Desireable properties
- Precisely specify what algorithms can provide for clients
- Separate algorithm implementation from client code
- Develop layers of abstraction, where we amke use of well-understood algorithms to develop other algorithms
### Types
1. Brute force
    - Time - high
    - Space - depends
3. Greedy
    - Time - O(n)
    - Space - depends
4. Divide and concure
    - Time - O(nlogn)
    - Space - high
6. Dynamic programming
    - Time - polynominal
    - Space - Use memoization

### Examples
1. Euclidian's Algorithm - find GCD of two numbers
2. Newton's method - numerical approximation
3. hypotenuse of right triangle
4. Sieve of Eratosthenes - primarlity test
5. hermonic number
6. Basic: 
    1. Operators
    2. Statement: declaration, assignment
    3. conditional, loops, calls, returns
7. Arrays:
    1. maximum/average/minimum of array
    2. copy to another array
    3. reverse order
    4. matrix-matrix multiplication
    5. dot-product
8. Recursion
    1. Base case (always first in a function)
    2. Subproblems that are smaller and do not overlap (subproblems should be disjoint)
    3. Proff by induction
    4. They lead to mathematical models that can be used to understand performance.
10. Search
    1. Binary search [p. 46]
11. Sorting
12. Graph


## Data structures
1. Primitive (Number, Boolean, Char)
2. String
3. ADTs
    1. Array
        1. linked list 
    2. Collections
        1. Stack
            1. Dikstras' two-stack expression evaluation
            2. FIFO
            3. LIFO
        3. Bag
        4. Queue 
            1. Priority Queue 
        5. Symbol Table
        6. Set
    3. Graph types
        1. (un)directed graph
        2. (un)weighted graph
        3. Opreation-oriented graph types
            1. Union-find
            2. (strongly) connected-components
            3. topological
            4. dfs path
            5. bfs path
            6. cycle search
            7. minimum spanning tree
            8. shortest paths

## Applications
1. whitelist filtering



# Data Abstraction
- **Data type** : set of values + a set of operations on those values.
- **Data abstraction** : process of defining and using data types.
- **Reference types** : allows for programming with the use of strings, pictures, sounds, or any other abstraction. A *reference* is a mechanism for accessing an object, i.e. a memory address.
- **ADT** : a data type whose representaion is hidden from the client. 
    - It supports encapsulation in program design.
    - **You cannot write code that depends on any specific representation in a ADT** E.g. the implementation might use `int` or `long`.

## Implementations
- Instance variables (*The state*)
- Constructors
- Instance methods (*The behaviour*), has a *signature* and a *body*
- Scope
    - there are *three* kind of variables: parameter, local and instance variables.

## Designing ADTs
- Use `private` access modifier on intance variables to made the class an ADT
- **Encapsulation** : 
    - allows for
        1. Independent development of client and implementation code
        2. Substitute improved implemenation without affecting client
        3. Support programs not yet written
    - isolates data-type operations, which leads to
        1. limiting the potential for error
        2. adding consistency check and other debugging tools in implmementations
        3. clarifying client code.
- Modular programming requires mainting *independence* among modules.
- **Designing APIs** : 
    - Takes practice, careful deliberation, and many iterations
    - Write every program as if you are going to reuse it again in the future; thus API
    - *Specification problem* : impossible to clearly articulate behavior for all possible imputs, including side effects
    - *Documentation* A brief English-language describtion of the  variable, constructor and methods including their side affects.
    - APIs may be : *too hard to implement*, *too hard to use**, *too narrow*, *too wide*, *too general*, *too specific*, *too dependent on a perticular representation*
    - *Motto* : ***"Provide to clients the methods they need and no others."***
    - *Algorithm* : typicaly a implementation of a instance method in an ADT.
    



# Function Abstraction
- **Function library** : in java, a set of static methods.


# Random
- Geometric objects are a good example of OOP. **Computational geometry** is its own field of study.
    - Point
    - Interval
    - Line 
    - etc.
- *Information processing*: abstract data types provides a natural mechanism for organising information, where the focus is encapsulation
- We rarely *fully* specify implementation requirements in an API.
# OOP principle
1. Specify an **API**: the purpose is to *separate client from implementation*
    1. First write the client code
    2. Implement the code that the client needs in API
        1. first the instance variables
        2. second the constructor
        3. third the instance methods 
2. Develop multiple test clients to validate the design desicion.

## Multiple implementaions
1. Identify different implementations of the same API by prepending a descriptive modifier. E.g.: `BasicDate`, `SmallDate`
2. Maintain a reference implementation with no prefix that makes a choise that should be suitble for most clients. E.g.:`Date`

# Goal
The goal of this book is to consider in depth several implementations of each of a number of fundemental ADTs, generally with different performance characteristics.

Multiple implemetaions of the same API can present *maintenance* and *nomenclature* issues. Any changes in an API once articulated might involve changing an unknown amount of client (and implemenation) code.