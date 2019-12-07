# CS 7200 Final Exam Guide
This guide will be made as a study tool for the final exam.  I will primarily be
using it to force myself to find and read the linked materials, and I would
recommend other students do the same, but feel free to use this as a reference
(please do not blame me for any grades earned by using this guide as a sole
reference)!


I will be starting this guide by documenting 2 things, the email sent
describing what will be on the exam, and the practice final on Dr. Prasad's
site.

Here are the topics on the final:
1. [Big Oh Recurrence (15
   pts.)](https://github.com/mkijowski/Algorithms-Final-Study-Guide/blob/master/README.md#big-oh-recurrence)
2. [Dynamic programming recurrence and algorithm use (10 pts)](https://github.com/mkijowski/Algorithms-Final-Study-Guide/blob/master/README.md#dynamic-programming)
3. [Skyline related question (10
   pts)](https://github.com/mkijowski/Algorithms-Final-Study-Guide/blob/master/README.md#skyline-problem)
4. [Classifying problems as tractable or intractable (10
   pts)](https://github.com/mkijowski/Algorithms-Final-Study-Guide/blob/master/README.md#intractability)
5. [Divide and Conquer Algorithm (5
   pts)](https://github.com/mkijowski/Algorithms-Final-Study-Guide/blob/master/README.md#divide-and-conquer-algorithm)

## Big Oh Recurrence
Oh yea...

## Dynamic Programming
Oh no...

## Skyline Problem
Review project submission

## Intractability
Review

## Divide and Conquer Algorithm
#### Master Theorem
Let T(n) be a monotonically increasing function that satisfies 

`T(n) = a T(n/b) + f(n)` 

`T(1) = c`  

Where a >= 1, b >= 2, c>0.  If f(n) is O(n^d) where d >= 0 

then
```
       {  O(n^d)                        if a < b^d
T(n) = {  O( (n^d)(log n) )             if a = b^d
       {  O( n^(log<sub>b</sub> a ))    if a > b^d
```

* master theorem is comparing the effort between the recursive splitting step
  (divide and combine), and the solution effort of the simplest case.
* fourth condition to Master theorem is applied in the closest point algorithm
* its not that master theorem doesnt apply to non-polynomial functions, we just
  cant prove that it does apply

#### Muster Theorem
Subtract and conquer, let T(n) be a function defined on positive n having the
property:

`T(n) = a T(n-b) + f(n)`

`T(1) = c`

Where a > 0, b > 0, d >= 0, and f(n) is in O(n^d).

then
```
        {  O(n^d)              if a < 1
T(n) =  {  O(n^(d+1))          if a = 1
        {  O( (n^d)(a^(n/b)) ) if a > 1
```


##### Deriving Master Theorem (and possibly Muster)
* First, learn the recursion tree method. Learn how to build the tree, how to count the number of leaves, and how to count the amount of "extra work" at each level, and how to sum them (by summing a series, e.g., a geometric series).
* Next, open up a textbook read a standard proof of the Master theorem. Work through each step and check that you understand what's happening.
* Now, close your textbook and put away all your resources. Put a blank piece of paper in front of you... and derive the Master theorem yourself. How do you do that? Well, you use the recursion tree method. Try working through it by yourself and try to solve the recurrence entirely on your own. If you get stuck, as a last resort you can open the textbook back up and see how to proceed from there... but then the next day, you should try this exercise again.

## Sample Midterm
###### 1) [Stable  Marriage  Problem]
State  whether  the  following  claims  are true  or false.   
If   true,   justify it as   clearly   as   possible. If false, provide a 
