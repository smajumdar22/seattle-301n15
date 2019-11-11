Reference - https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa

What is functional programming?
Functional programming is a programming paradigm — 
a style of building the structure and elements of computer programs 
— that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data —Wikipedia

Pure functions benefits
The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:
Given a parameter A → expect the function to return value B
Given a parameter C → expect the function to return value D
A simple example would be a function to receive a collection of numbers and expect it to increment each element of this collection.

We receive the numbers array, use map incrementing each number, and return a new list of incremented numbers.

For the input [1, 2, 3, 4, 5], the expected output would be [2, 3, 4, 5, 6].

Imuutability - 

When data is immutable, its state cannot change after it’s created. 
If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

Referential Transperancy - 
pure functions + immutable data = referential transparency
