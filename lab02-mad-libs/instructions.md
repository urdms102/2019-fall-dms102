# Lab 2: Mad Libs

Due: today (Tuesday, September 10, 2019)

This assignment tests your ability to create a simple, one-function program that requires user input to be used as arguments

## Create a *Mad Libs* Program with Parameters

Your task is to create a similar program as Program 11 in the book (page 48) with some differences as described below:

1. Create a Python file named: **lab02.py**

Edit the **lab02.py** file in JES as follows...

2. Add a three-line comment block (lines 1-3) to describe the program like this

```pyt
# ********************
# Customized Program 11: Original Mad Lib Story with Parameters
# ********************
```

3. Then write your own, original Mad Lib story with the following differences:
   - Give the function a unique name - something that relates to the story you're going to write (*not* `madlib3()` as shown in the book)
   - Write your own, original story (don't copy what's in the book); you can use anywhere between 5 to 10 lines
   - Use at least five or more parameters (not four as shown in the book)
   - Make sure all the lines print out (as shown in the book) at the end of the function. (It's doesn't matter how many lines of code you use to print out all the lines.)

4. Below the program, add a "TEST" block (with a three-line comment block, like we did in Lab 1)
5. In the test block, write code to ask the user for input using the `raw_input()` function like this:

```put
animal1 = raw_input("Enter a type of animal: ")
```

…do this for each argument you'll need to run the program.  I.e. if you created a program that requires five parameters, you'll need to use the `raw_input()` function five times with appropriate prompts and variable names.

6. Run the program using the arguments you created.  Here's an example of a program, named `mittensStory()` that requires seven arguments:<br>`mittensStory(animal1, name, adjective, food, animal2, place, furniture)`

REQUIRED: When the program prints its output, the spacing of the words must be correct, i.e. no extra spaces or words smushed together in the middle of the paragraph.  

Also, to the best of your ability, you must make the story make sense, however getting all combinations of input to make perfect semantic sense is hard.  Don't worry about that.


### Turn-in the Assignment for Credit

1. When your program is working correctly, open a web browser and navigate to our DMS 102 section in Blackboard; in the "Lab Assignments" area find "Lab 2: Mad Libs"
3. Upload your **lab02.py** file to the Lab 2 assignment

