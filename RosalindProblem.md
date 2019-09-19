# Transcribing DNA into RNA

Bioinformatics is the science of collecting and analyzing complex biological data such as genetic codes.
In order to broaden your horizons and show that the concepts you have been learning can be applied almost anywhere, 
we are going to be converting a DNA strings to RNA strings using for loops!

DNA is a string of genetic code composed of two sequences (strings). These strings are composed
of the characters A G T and C where A matches with T, and C matches with G. 
In any DNA gene based expression such as the creation of protiens in the cell, a process called 
DNA Transcription occurs in which the DNA is unwound, seperated in a section into 2 strands and an
enzyme called RNA Polymerase begins constructing a complimented strand of Genetic code called RNA.
This strand will be identical to the compliment DNA strand that was unwound except for there wont be 
and T's, instead there will be U's. 

Given this information:

1. take in the user's DNA "string" as a string of A's, T's, G's, and C's
2. loop over the input string
3. conditionally check each character and compose a compliment RNA string to the user's input string.
4. Print out the resulting RNA string back to the user as follows:

`The compliment to the DNA string (Your DNA String) is (Your RNA String)`

Remember that the basic structure of a for loop is as follows:

```

list A = ['a', 'b', 'c']

for item in list: (item will = 'a', then 'b' etc.)
  do something
  
```

If the user entered a character that cannot be recognized and converted to RNA, 
we will want to tell the user there was an error and promptly quit running.
To do this, we can use the sys library in python, No need to get in depth on libraries
at this time but using the following code, you can exit a program whenever and wherever 
if needed.

```

import sys
...
sys.exit()

```

# Sample Output

```
Enter a DNA String:
>>> ACGTGTACCAGGT
For the DNA String ACGTGTACCAGGT The compliment RNA String is UGCACAUGGUCCA
```

```
Enter a DNA String:
>>> ABCDE
B is not a valid input character
```

