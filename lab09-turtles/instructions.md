Lab 9: Turtles
====================

*Due: Thursday, December 5, 2019 (today, by 3:15 PM)*

For this in-class lab exercise, you need to use the built-in Turtle objects and its related methods to write your initials (at least three) in a "World"

Note: this lab is timed - due by the end of this class period (3:15 PM).  Labs turned-in late but before 9:00 PM that time will lose 10 points.  Labs turned-in later than that will lose 20 points.

## Requirements

- [ ] Create a file called **lab09.py** in which you'll write the program

- [ ] Write a program that writes your initials
- [ ] Separate your initials with some space in-between each letter
  - Hint: use the methods `.penUp()` and `.penDown()`
- [ ] Have your turtle rest briefly between each pen stroke
  - Hint: import the `sleep` function from the `time` library

- [ ] Required: use a class named `MyTurtle()` that extends the Class "Turtle"

Here's how to setup the Class.  (Notice: you're creating a sub-class because **MyTurtle** uses Turtle as a parameter, so everything a Turtle "knows" your MyTurtle will know too.)

```python
class MyTurtle(Turtle):
  #start setting up methods here...
```

- [ ] Required: use a test case to instantiate a World and instantiate your Turtle in that World 

Here is an example test case to instantiate a World and instantiate a MyTurtle in that World

```python
# TEST
earth = World()
me = MyTurtle(earth)
#suggestion: create a method named .drawInitials() and use that
#  to call other methods that actually draw the letters
me.drawInitials()
```

### Turn-in the Assignment for Credit

- When your program is working correctly, upload your **lab09.py** file to **Lab 9: Turtles** into the "Lab Assignments" area in our DMS 102 section in Blackboard
  - You do not have to ZIP (compress) this file

