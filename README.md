# LeetCode (30 Days of JavaScript)

## About the problem
- *Problem Number* : 2667
- *Problem Name* :  [Create Hello World Function](https://leetcode.com/problems/create-hello-world-function/)
- *Problem difficulty* : Easy 🟢
- *Programming language used* - JavaScript

## Problem

Write a function createHelloWorld. It should return a new function that always returns "Hello World".
 

Example 1:

Input: args = []
Output: "Hello World"
Explanation:
const f = createHelloWorld();
f(); // "Hello World"

The function returned by createHelloWorld should always return "Hello World".
Example 2:

Input: args = [{},null,42]
Output: "Hello World"
Explanation:
const f = createHelloWorld();
f({}, null, 42); // "Hello World"

Any arguments could be passed to the function but it should still always return "Hello World".
 

Constraints:

0 <= args.length <= 10


## Approach Explanation
Solved using high order function 👍

### If you have suggestions for improvement or would like to contribute to this solution, feel free to create a pull request. 🙌😇
