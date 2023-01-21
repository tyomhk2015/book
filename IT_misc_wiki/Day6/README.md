<a href="https://github.com/tyomhk2015/book/tree/main/IT_misc_wiki" rel="noopener noreferrer"><b><< Back</b></a>

# Day 6

From chapter 26 to 29.



### Chapter 26

<b><i>Sorting algorithms</i></b>

Though some algorithms have same Big-O-Notations, this does not mean that the performance or speed of those algorithms are exactly same. Some algorithms are operated more efficiently than the others.

For instance, bubble sort, selection sort, and insertion sort have the same big-O-Notation, `O(N^2)`.

The selection sort has better speed because the number of looking at the index of the given array, and comparing the values in specific index, are lesser than the bubble sort.

The insertion sort has better performance than the bubble and selection sort, despite the same big-O-Notation. 

Why is there practical performance differences when they have the same big-O-Notation? 

The reason is the prerequisites or some conditions are prepared in ahead of checking the big-O-Notation, like the minimum and maximum values are known in advance.


### Chapter 27

<b><i>The terms of `queue` and `stack`.</i></b>

Both are abstract data type. Unlike an array, which has its syntax in any language, `queue` and `stack` do not have its own syntax. They are just specifications or some rules to follow, and can be built using an array.

Stack = Last in, First out.
Queue = First in, First out.


### Chapter 28

<b><i>What is `hash table`?</i></b>

Data that is consist of `key` and `value`, just like a dictionary.

Hash tables consists of an array and a `hash function`. This `hash function` translates given `key` into a hash code, and this hash code can be used to search specific element of an array.

If there is no `hash collison`, the performance of the hash tables may be seen as `O(1)`. However, if there is a `hash collison`, the time complexity for searching the specific value may be `O(N)`, but this depends on what kind of hash function is being used. 

`Hash collison` is an occurence of producing same hash when two different inputs are given to the hash function. One of solutions of this is the hash function runs linear search of the array that the hash code is pointing at, until the function finds the proper `value` the given `key` was looking for.


### Chapter 29

<b><i>Clean code</i></b>

Practices of writing code for maintanance and readability.

Five of those pratices are elaborated in the book.

```
  1. The name of the variables or functions should have meaningful words.
  2. The name of functions should start with a verb.
  3. Reduce the number of arguments for a function.
  4. Do not use a boolean type as an argument.
  5. Do not over-abbreviate words.
```

I agree with number 1, 2, 3, and 5, but not 4.

```
  #1, #2
```

While I was working at Recruit Co., Ltd., as a frontend dev, I had to maintain a legacy project that was using jQuery, and the some variables and functions were not abiding to the `clean code`. I fixed those meaningless names with names that represent the variables' or the functions' role.

```
  #5
```
The story continues with the same company I mentioned above. Once the variables names were to short that I could not get the meaning in an instance. Changed those over-shorted names to original words and got rejected in code review. The reason was that the company wanted to keep the names short. Well, they are the boss of their products, I reverted all the names back to over-shorted ones.

For instance, `err` to `error`, or `uid` to `userID`.

Honestly, I believe that comment or documentation must be left even though the code is written in `clean code` style, because the we cannot convey the philosophy or the intention of writing the specific code for some features. Even many third-party libraries the Google Chrome is using, have good comments in the code base while keeping their code as clean as possible.

<hr>

 #노마드코더 #북클럽 #노개북