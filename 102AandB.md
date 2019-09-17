# Lost Your Marbles

In the previous labs, we've discussed looping using `while`. 
In this lab we will be furthering our knowledge of loops by using `for` loops.
What will we be doing with these loops you may ask? Finding our marbles of course!

## Problem Statement
We've lost our marbles! Unfortunately for us, the lights went out at the same time and 
we would have a bit of trouble searching for all our marbles. One thing we do know is that 
they have fallen onto a grid of `X's` and we can use a small bit of code to help us 
find out where all of them are while we go do anything more productive than 
sort through a pile of pieces one by one.

For the first part of the lab, you will be seaching for the location of all Marbles `(O's)` 
randomly throughout a string of `X's`.

A sample input may look something like the following:
`"XOXXXOOXXXXOOOOXXXXXXXOOOOOOX"`

Your Program may be structured as follows:
- Prompt the user for a "random" string of X's an O's. **(Note: O as is the letter O not the number 0)**
- Convert the input string to lowercase or upercase using the `lower()` and `upper()` functions. This will 
prevent accidental caps typo's (*Note: A != a to a computer, the letters are the same, but their Ascii value is different*)

```
Example
str = input( ...... ).lower()
```

- Create a variable to keep track of the index of the string as you iterate over it and an empty list to store 
your identified marbles in.
- Iterate over the values of the input string
- Using `conditionals` check to see:
  - If value is a Marble then store the current index in your running list of marble locations
  - Otherwise the value is an X, do nothing
- Incriment your index counter to keep track of the new index

Once the loop completes we should have a running list of all the locations of our marbles. Display that 
list and the number of marbles found back to the user with a witty message such as:

`Hi Lazy, I found your marbles for you, they are at [0, 2, 4, 10, 12, 16]`

### Sample Output
```
```

# But Wait!
It was nice that the first time we dropped all our marbles onto a grid with only one row, but what 
happens when we really lose our marbles, they go all over!

For part B of this Lab, you will be creating and iterating over `2d Lists`!!! (2 Dimensional) This process is 
extremely useful in things like image processing, image recognition, matricies, etc.

The Goal for `Part B` is the same as for `Part A`, except you with be working not only in the x 
direction, but also the y. We won't be using user input this time as one wrong letter could mess
with the construction of our 2d list. So first things first, lets make a 2d list. 

Conceptually, a 2d list is a list, where all of it's values are also lists of some other value.
Choose a value `n` less than 10 for simplicity and construct a list, containing `n` strings of length 
`n` containing only `X's` and `O's`.

*The following shows an example of what you are trying to construct conceptually, but not actual code*

```
 X X X O X X X X O X
 X X X X X X X X X X
 X X X X X O X X X X
 X X X O X X X X X X
 X X X X X X X O X X
 X X X X X X X X X X
 X X X X X O X X X X
 X O X X X X X X X X
 X X X X X X X O X X
 X X X X X X X X X X
 ```
Based on `Part A` we know how to use a `for` loop to go through a `String` and find values within,
so if we set all of that inside another `for` loop, we should be able to go through each row, then each column,
searching for our marbles. Be sure to keep track of index's.

You will need to create a tuple `tuple` (*A collection which is ordered and unchangeable)
containing the x,y position of the marble within the 2d array and add that tuple to a list that will be 
printed out to the user when the grid completes it's iteration.

Tuples can be created as such
```
x = 5
y = 6
t = (x,y)
print(t)

> (5,6)
```

Sample Output
```

```
