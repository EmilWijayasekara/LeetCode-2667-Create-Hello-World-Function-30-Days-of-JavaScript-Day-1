# LeetCode (30 Days of JavaScript)

## About the problem
- *Problem Number* : 13
- *Problem Name* :  [Roman to Integer](https://leetcode.com/problems/roman-to-integer/)
- *Problem difficulty* : Easy (60.01%) 🟢
- *Category* : Algorithms
- *Programming language used* - Java

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
I've approached this problem by iterating through the Roman numeral string from `right to left`. 
For each numeral, I use a switch statement to map it to its corresponding numerical value, or this can be done using a HashMap also.

I used three variables which are:
```cpp
int correspondingNaturalNumber = 0;  
int answer = 0;  
int previous =0;
```
`previous` variable used to get the previous number currently iterating through.
`answer` is final return value that i added all roman number values.
`correspondingNaturalNumber` in switch statement i mapped roman number to natural numbers.

After that using if else statement, I compare the current numeral's value (`correspondingNaturalNumber`) with the value of the previous numeral (`previous`). If the current numeral is smaller than the previous one, its value is subtracted from the result; otherwise, it is added.

After processing each numeral, I update the `previous` variable to store the current numeral's value. This ensures that the correct value is considered in the next iteration.

### If you have suggestions for improvement or would like to contribute to this solution, feel free to create a pull request. 🙌😇
