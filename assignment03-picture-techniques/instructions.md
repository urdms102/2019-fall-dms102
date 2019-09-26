# Assignment 3: Picture Techniques

Due: Thursday, October 3, 2019 (one week)

This assignment tests your ability to target individual pixels and change their color based on some criteria.

## Requirements

The goal is to write a program that targets one area of a digital photograph and changes a range of colors within that area to another color

- [ ] The program must be generic enough to work with ANY digital photograph (a "picture object"), i.e. the picture must not be hardcoded into the program
- [ ] The program must be generic enough to target ANY area within the digital photograph, i.e. the coordinates must not be hardcoded into the program
- [ ] The program must be generic enough to target ANY color within ANY range (i.e. distance) within the targeted area in the digital photograph AND the color that's targeted can be changed to ANY other color (...again, that means none of this information can be hardcoded in the program)
- [ ] The program must "return" the picture object

Hint: the requirements above mean you'll need to use A LOT of parameters in the function!  Those parameters will include:

- A picture object
- Four coordinates: `startX`, `startY`, `endX`, and `endY`
- A color object (can be a keyword or a variable created using `makeColor()`
- A color distance (a single integer between 0 and 441)
- Another color object (can be a keyword or a variable created using `makeColor()` to create the "end Color"

You will also need to create a TEST case to run your program.  The requirements for the TEST:

- [ ] It should start with `setMediaPath()` and then hardcode the file name of your digital picture (which you will provide when you submit this assignment in Blackboard) 
- [ ] It should create a picture object from the digital picture
- [ ] The program should be called using your picture object as an argument, plus all the other parameters required to run the program
- [ ] When the program is called, it must capture the returned picture object and then...
- [ ] Write the picture object to the hard drive using a new filename (hint: use `writePictureTo()`)
- [ ] "Explore" the picture object






### Turn-in the Assignment for Credit

1. When your program is working correctly, open a web browser and navigate to our DMS 102 section in Blackboard; in the "Lab Assignments" area find "Assignment 3: Picture Techniques"
3. Upload your **assignment03.py** file and the image files (original and altered) to Blackboard

