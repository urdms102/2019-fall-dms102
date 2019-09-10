# Assignment 1: Palindrome

Due: Thursday, September 12, 2019 (before the next class starts)

This assignment tests your ability to take a palindrome entered by the user, and print it out forward and backwards so they look identical, like this example...

```python
>>> 
======= Loading Program =======
Palindrome: A Man, A Plan, A Canal, Panama!
Forward:    amanaplanacanalpanama
Backward:   amanaplanacanalpanama
>>> 
```

General Requirements:

- [ ] The program must pause for the user to enter a palindrome using the `raw_input()` function
- [ ] The text that follows the three labels must line-up (simply add spaces to the labels to get that to work)
- [ ] There are many ways to code this program, however you must try to optimize the code to as few lines as possible

Other Requirements for the "Forward" and "Backward" text:

- [ ] All characters must be converted to lowercase
- [ ] All spaces and punctuation must be removed
- [ ] When a true palindrome is entered by the user, the text - forward and backward - must be identical

See Program 20 in the book (page 55) as a starting point:

1. Create a Python file named: **assignment01.py**

Edit the **assignment01.py** file in JES as follows...

2. Add a three-line comment block (lines 1-3) to describe the program like this

```pyt
# ********************
# Customized Program 20: Palindrome
# ********************
```

3. Then using Program 20 as a starting point, create a customized version of that program that creates output like shown in the example, above.
   - [ ] Required: the name of the function must be `palindrome()` (not "reverse")
   
4. Below the program, add a "TEST" block (with a three-line comment block)

5. Below the test block, write code to ask the user for input using a prompt like this:<br> `input = raw_input("Enter a Palindrome: ")`

6. Then run the program using the `input` from the user

## Hints & Tips

- Although it might not be necessary depending on how you code your program, you *may* use two "pile" variables (like `pile1` and `pile2` or something like that) to build the "forward" and "backward" piles
  - Also note, the pile variables do not need to be named "pile" at all; it would be great if you come up with variable names that make more sense for what you're doing

- You can filter out the spaces and punctuation using the `if not` statement as shown in Program 16
  - You do not have to filter out every possible punctuation mark - just the most common like: commas, periods, exclamation marks, question marks, ...stuff like that
- You can convert all the characters to lower case using the `.lower()` method as shown in Program 18


### Turn-in the Assignment for Credit

1. When your program is working correctly, open a web browser and navigate to our DMS 102 section in Blackboard; in the "Labs and Assignments Turn-in" area find **Assignment 1: Palindrome**
3. Upload (attach) your **assignment01.py** file and click the Submit button
