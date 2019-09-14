---
layout: post
title:      "Recursion Explained With Example"
date:       2019-09-04 21:27:47 -0400
permalink:  recursion_explained_with_example
---


Most programmers have heard of this concept and fear it. They tend to stay away from it. It is a scary subject but it doesn't have to be! It took weeks until it clicked for me, hopefully I can speed that process for others. To really understand **recursion**, you have to open your mind to different ways of thinking and solving problems.

## What is recursion?

Recursion is when a function  calls itself. I know that sounds strange. When one is coding, its very unusual for you to make a function call itself, but it can be useful. It often comes up in binary search trees. Here is an example of recursion for a simpler problem:

```
//Returns the sum of all numbers from 0 to a given integer
function sumRange(num){
    if (num === 0){
        return 0
    }
    
    return num + sumRange(num -1)
}
```

The important thing to keep in mind about recursion is that it is a **different** way of thinking. The code doesn't get solved from beginning to end, it actually solves from the end backwards. Here is how the computer would solve it:


![Recursion Gif](https://i.imgur.com/TCzJil7.gif)


This is how the computer would solve a problem recursively. Hopefully I didn't lose you there. The good thing about this, is you don't actually have to solve iteration by iteration, you just give the function a pattern to follow.

I will explain the mindset of thinking recursively. Let's look back at the code. 


```
//Returns the sum of all numbers from 0 to a given integer
function sumRange(num){
    if (num === 0){
        return 0
    }
    
    return num + sumRange(num -1)
}
```

You can divide the code into 2 parts:

1- Base Case. 

```
 if (num === 0){
        return 0
 }
```

This is where your pattern ends. In this case, we added all numbers from 0 to an integer. It doesn't matter if the integer is 1, 10, or 100, we will always add every number, stopping when we reach to 0.

2- Main pattern

```
return num + sumRange(num -1)
```

This is where the function will call itself based on the pattern of the particular problem. It's very common for the function to call itself each time with a **smaller** and **smaller** number, until it eventually reaches your **base case**. In this case, we called the function again with the same number minus one. The number will always keep getting smaller until it reaches our **base case**, 0.

That's all there is to recursion. To **think recursively**, is really to think of a problem and divide it in two things: What is its base case? And what is its pattern?

