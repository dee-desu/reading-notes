
# Read 03 - Whiteboarding + Big O

### What is Big O notation?

Big O notation is a mathematical notation that describes the limiting behavior of a function when the argument tends towards a particular value or infinity. It is a member of a family of notations invented by Paul Bachmann, Edmund Landau, and others, collectively called Bachmann–Landau notation or asymptotic notation.”
![image](https://www.freecodecamp.org/news/content/images/2021/06/1_KfZYFUT2OKfjekJlCeYvuQ.jpeg)<br><br>
---
### O(1)
The first Big O Notation that we have is O(1), it simply means that the operation will always execute in a constant amount of time regardless of how big the input size is.

### O(n)
Describes an algorithm performance will grow linearly and in direct proportion to the size of the input data set.

### O(N^2)
the number of operations it performs scales in proportion to the square of the input. This is common with algorithms that involve nested loops or iterations.

### O(2^n) 
it denotes an algorithm whose growth doubles with each addition to the input data set.
The growth of this algorithm is exponential, let’s say we have n=2 inputs, then it will perform 4 times, with n=3, it will perform operations 8 times and so on.

### O(log n)
basically means time goes up linearly while the n goes up exponentially. So if it takes 1 second to compute 10 elements, it will take 2 seconds to compute 100 elements, 3 seconds to compute 1000 elements, and so on.
