# Assignment 3: Picture Techniques

Due: Thursday, October 3, 2019 (one week)

This assignment tests your ability to target individual pixels and change their color based on some criteria.

## Requirements

The goal is to write a program that targets one area of a digital photograph and have it change a range of colors within that area to another color

- [ ] The program must be written in a single Python file named **assignment03.py**
- [ ] The program must be abstract enough to work with ANY digital photograph (a "picture object"), i.e. the picture must not be hardcoded into the program
- [ ] The program must be abstract enough to target ANY area within the digital photograph, i.e. the coordinates must not be hardcoded into the program
- [ ] The program must be abstract enough to target ANY color within ANY range (i.e. distance) within the targeted area in the digital photograph AND the color that's targeted can be changed to ANY other color (...again, that means none of this information can be hardcoded in the program)
- [ ] The program must "return" the picture object

Hint: the requirements above mean you'll need to use A LOT of parameters in the function!  Those parameters will include:

- A picture object
- Four coordinates to deliniate a rectangle on the picture (hint: four separate parameters)
- A color object (can be a keyword or a variable created using `makeColor()`)
- A color distance (a single integer between 0 and 441)
- Another color object (can be a keyword or a variable created using `makeColor()` to create the "end Color")

You will also need to create a TEST case to run your program.  The requirements for the TEST:

- [ ] It should start with `setMediaPath()` and then hardcode the file name of your digital picture (which you will provide when you submit this assignment in Blackboard) 
- [ ] It should create a picture object from the digital picture
- [ ] The program should be called using your picture object as an argument, plus all the other parameters required to run the program
- [ ] When the program is called, it must capture the returned picture object and then...
- [ ] Write the picture object to the file system using a new filename (hint: use `writePictureTo()`)
- [ ] Last step: "explore" the picture object

*Another requirement for the TEST:*
- [ ] The TEST needs to demonstrate the program in an interesting way, i.e. something that looks purposeful 
  - Example: changing a yellow flower to blue; changing the blue sky to black
  - Note: if the area selected on your picture looks random, for example if it bisects an object in your photo in a way that doesn't make sense, points will be deducted

## Extra Credit

The output of this assignment generates a new digital picture file.  If you can write another program in the same Python file that accepts that digital picture file as an argument and then "posterizes" it and generates another new digital picture file, you will receive:

- At the end of the semester, your lowest assignment grade will be dropped

Note: for the extra credit, you must also append the TEST block to run your posterization program and write another digital picture file to the file system


## Turn-in the Assignment for Credit

- When your program is working correctly, open a web browser and navigate to our DMS 102 section in Blackboard; in the "Labs and Assignments Turn-in" area find **Assignment 3: Picture Techniques**
- Upload your **assignment03.py** file and the image files (original and altered) to Blackboard

