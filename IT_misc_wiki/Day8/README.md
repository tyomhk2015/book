<a href="https://github.com/tyomhk2015/book/tree/main/IT_misc_wiki" rel="noopener noreferrer"><b><< Back</b></a>

# Day 8

From chapter 35 to 38.



### Chapter 35

<b><i>How passwords are saved?</i></b>

Hash function encrypts the password into unreadable text. For better security, and to prevent from being decrypted by `rainbow table`, `salt` is added to the hashed password.

```
  Hash function
```
A tool that changes the input value to some random characters. Same input will produce same output, but not vice versa.


```
  Rainbow table
```
A record of what hash function's outputs are depending on the input. Main purpose of the table is to find encrypted passwords.

```
  Salt
```
Small amount of random characters that are appended to original password before hashed.

### Chapter 36 & 37

<b><i>OOP</i></b>

Object oriented programming.

One of many practices of writing and maintaining code.
Usually uses `class`, `inheritence`. In context of time efficiency and maintainability, OOP are better than procedural programmng.



### Chapter 38

<b><i>Functional programming</i></b>

One of many practices of writing and maintaining code. Codes are mostly written using functions, e.g. React.js.

- Imperative programming: Describes the detail of computation.
- Declarative programming: Describes the flow of the logic.

<hr>

 #노마드코더 #북클럽 #노개북