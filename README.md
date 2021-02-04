# Arrays

## Arrays Resources

To brush up on arrays, check out the resources below.

1. _Grokking Algorithms_ by Aditya Bhargava is a must-read if you’re prepping for interviews. It is not language specific. Check out [Chapter 2, Selection Sort](https://livebook.manning.com/book/grokking-algorithms/chapter-2/)
2. Recommended chapters from Allen B. Downey’s free computer science textbooks.
    * _Think Data Structures_ is a general text about data structures that is not language specific. Check out [Chapter 2, “Analysis of Algorithms”](http://greenteapress.com/thinkdast/html/thinkdast003.html) and [Chapter 3, “ArrayList”](http://greenteapress.com/thinkdast/html/thinkdast004.html)
    * _Think Python_ is a successor to “How To Think Like A Computer Scientist,” specific to Python. If you’d like to think about arrays in Python, check out [Chapter 10, “Lists”](http://greenteapress.com/thinkpython2/html/thinkpython2011.html)
    * _Think Java_ is the Java version. If you’d like the Java perspective, check out [Chapter 8, “Arrays”](http://greenteapress.com/thinkjava6/html/thinkjava6009.html)
3. _Harvard CS50 Lectures, 2019_ is a great place to start learning. The demonstration language is C, but you don’t need to know C to follow along. If you expand the bar just below the video window, where it has the picture of the cat for CS50, you can see links to specific timestamps. [Arrays are at 08:44](https://www.youtube.com/watch?v=4IrUAqYKjIA&t=524s)_

# LeetCode Problem Set 

- [ ] [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/) & [My Solution](https://github.com/ChandaHubbard/leetcode/blob/master/53.%20Maximum%20Subarray.md)
- [ ] [54. Spiral Matrix](https://leetcode.com/problems/spiral-matrix/) *
- [ ] [881. Boats to Save People](https://leetcode.com/problems/boats-to-save-people/) 
- [ ] [1266. Minimum Time Visiting All Points](https://leetcode.com/problems/minimum-time-visiting-all-points/) *
- [ ] [1394. Find Lucky Integer in an Array](https://leetcode.com/problems/find-lucky-integer-in-an-array/) *
- [ ] [1395. Count Number of Teams](https://leetcode.com/problems/count-number-of-teams/)

# Techniques to solve problems using arrays


## 1. Implement an Array class from scratch.
Walk through each step of implementing an array. Don't rush through this by copying and pasting the code samples. After you've walked through it and you understand the code of the Array class, hide the sample code and try writing the Array class from scratch using the memory module here for allocating memory.

Be sure to export the memory module and then import it using require.

## 2. Explore the push() method
Using the Array class you just created above, add an item to the array. Use the following function:

```
function main(){

    Array.SIZE_RATIO = 3;

    // Create an instance of the Array class
    let arr = new Array();

    // Add an item to the array
    arr.push(3);

    console.log(arr);
}
```
What is the length, capacity and memory address of your array?

Add the following in the main function and then print the array:
```
    ...
    arr.push(5);
    arr.push(15);
    arr.push(19);
    arr.push(45);
    arr.push(10);
 ```
    
What is the length, capacity and memory address of your array? Explain the result of your program after adding the new lines of code.
## 3. Exploring the pop() method
Add the following in the main function and then print the array:

 ``` 
  ...
  arr.pop();
  arr.pop();
  arr.pop();
 ```
 
What is the length, capacity, and address of your array? Explain the result of your program after adding the new lines of code.

## 4. Understanding more about how arrays work
Print the 1st item in the array arr.

Empty the array and add just 1 item: arr.push("tauhida");

Print this 1 item that you just added. What is the result? Can you explain your result?

What is the purpose of the _resize() function in your Array class?

You can use JavaScript's built-in arrays to solve the following drills. After you write the algorithm, identify its time complexity and determine if it needs to be optimized. Start each problem by understanding the problem and coming up with some sample input and output. For your convenience, a few sample input and output are provided.

## 5. URLify a string
A common mistake users make when they type in an URL is to put spaces between words or letters. A solution that developers can use to solve this problem is to replace any spaces with a %20. Write a method that takes in a string and replaces all its empty spaces with a %20. Your algorithm can only make 1 pass through the string. Examples of input and output for this problem can be

Input: tauhida parveen

Output: tauhida%20parveen

Input: www.thinkful.com /tauh ida parv een

Output: www.thinkful.com%20/tauh%20ida%20parv%20een

## 6. Filtering an array
Imagine you have an array of numbers. Write an algorithm to remove all numbers less than 5 from the array. DO NOT use Array's built-in .filter() method here; write the algorithm from scratch.

## 7. Max sum in the array
You are given an array containing positive and negative integers. Write an algorithm which will find the largest sum in a continuous sequence.

Input: [4, 6, -3, 5, -2, 1]
Output: 12

## 8. Merge arrays
Imagine you have 2 arrays which have already been sorted. Write an algorithm to merge the 2 arrays into a single array, which should also be sorted.

Input:[1, 3, 6, 8, 11] and [2, 3, 5, 8, 9, 10]
Output:[1, 2, 3, 3, 5, 6, 8, 8, 9, 10, 11]

## 9. Remove characters
Write an algorithm that deletes given characters from a string. For example, given a string of "Battle of the Vowels: Hawaii vs. Grozny" and the characters to be removed are "aeiou", the algorithm should transform the original string to "Bttl f th Vwls: Hw vs. Grzny". Do not use Javascript's filter, split, or join methods.

Input:'Battle of the Vowels: Hawaii vs. Grozny', 'aeiou'
Output: 'Bttl f th Vwls: Hw vs. Grzny'

## 10. Products
Given an array of numbers, write an algorithm to find out the products of every other number except the number at each index.

Input:[1, 3, 9, 4]
Output:[108, 36, 12, 27]

## 11. 2D array
Write an algorithm which searches through a 2D array, and whenever it finds a 0 should set the entire row and column to 0.

Input:
[[1,0,1,1,0],
[0,1,1,1,0],
[1,1,1,1,1],
[1,0,1,1,1],
[1,1,1,1,1]];
Output:
[[0,0,0,0,0],
[0,0,0,0,0],
[0,0,1,1,0],
[0,0,0,0,0],
[0,0,1,1,0]];

## 12. String rotation
Given 2 strings, str1 and str2, write a program that checks if str2 is a rotation of str1.

Input: amazon, azonma

Output: False

Input: amazon, azonam

Output: true
