
# FUNCTIONAL PROGRAMMING
Functional Programming is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

In other words, the program should return new data without modifying the original data.



# pure functions
The first fundamental concept we learn when we want to understand functional programming is pure functions.

It returns the same result if, given the same arguments (it is also referred to as deterministic), It does not cause any observable side effects

If our function reads external files, it’s not a pure function — the file’s contents can change

Any function that relies on a random number generator cannot be pure.

It does not cause any observable side effects . Examples of observable side effects include modifying a global object or a parameter passed by reference.



# Pure functions benefits
Immutability
Unchanging over time or unable to be changed. When data is immutable, 


# Refactoring JavaScript

It's important to get your code right the first time because in many businesses there isn't much value in refactoring. Or at least, it's hard to convince stakeholders that eventually uncaged for codebase will grind productivity to a halt.

Filter :The filter function expects a true or false value to determine if the element should or should not be included in the result collection.

Map : transforms a collection by applying a function to all of its elements and building a new collection from the returned values.

Reduce :to receive a function and a collection, and return a value created by combining the items.

