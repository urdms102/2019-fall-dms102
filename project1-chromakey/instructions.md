# Project 1: Chromakey

Due: Tuesday, November 19, 2019

The goal of this project is to create a single picture that demonstrates the use of chromakey background substitution, with particular attention on lighting conditions to make sure the result looks as natural as possible even if the subject matter could not exist in real life.  

The creation of the picture with the substituted background must be accomplished using Python.  

## Step 1: Foreground

- Take a picture of a person(s) or other subject matter in front of a chromakey-green background
  
  - Take note of the type of lighting used: temperature (in Kelvin); and direction

## Step 2: Background

- Take a picture of a landscape or similar outside subject that will be used as the background to the foreground picture
- The lighting conditions of the background must match the lighting used in the foreground picture (temperature and direction)

## Step 3: Merge

- Using Python (specifically Jython in JES), write a sufficiently abstracted program that substitutes the chromakey background in the image from Step 1 with the image from Step 2.

## Rubric

The merged image must meet the following criteria, as well as possible.

##### General Requirements

- [ ] Both pictures (from Step 1 and Step 2) must be original, taken by you, the student, this semester - not from the Internet nor any other source
- [ ] The subject matter must look well-thought out and planned, indicating some level of forethought and creativity; humor is strongly encouraged

##### Photographic Quality

- [ ] The lighting in the merged picture must look natural as if both the foreground and background we're photographed in the same location at the same time, even if the result is impossible
- [ ] In the merged picture, to the greatest extent possible, there must be no chromakey pixels from the foreground picture AND to the greatest extent possible, there must be no accidental "drop outs" of the subject matter from the foreground picture

##### Programming Requirements

- [ ] The substitution of the chromakey-green background from the foreground image must be totally accomplished **in JES using Jython**
- [ ] The program must demonstrate a sufficient level of **abstraction**, meaning the program you write cannot have hard-coded picture objects nor unique values to merge the two pictures; specifics that will be used to merge your actual two pictures must be passed-in to your program using parameters
- [ ] Because your program will be abstracted, you must also provide a use case (i.e. **a TEST block**) where your two picture files with be hard coded, along with the specific values they need to have applied to successfully swap-out the chromakey-green with the new background
  - NOTE: when grading, the professor will attempt to run your program on your provided picture files to regenerate the same results you got.  ALSO, the professor will use his own test case and different images on your program to test for abstractness.  

## Hints & Tips

- When doing the merge, the foreground picture will be placed in the top-left (the 0,0 pixel) of the background picture, therefore the size (dimensions, in terms of height and width) of **the background picture needs to be at least the same or larger** than the foreground picture
- You may prepare the foreground and background pictures using any picture editing software (like **Photoshop, GIMP, whatever**) to resize and fine-tune them before merging them together.  HOWEVER...
- You may NOT alter the chromakey-green of the foreground picture in any way before merging the two pictures using Jython in JES.  The actual background replacement process must be done using a program that you write in Jython.
- The program you write may be based on the program shown in the book: **Program 58: Chromakey Green**, however you'll find that the algorithm used in that example (specifically, the IF statement in the fifth line) might not work well.  Suggestion: try a different algorithm, perhaps using the `distance()` function to select the green pixels better.  Also note, you will probably have to change more than the IF statement (line 5) to get the best possible results.  

## Turn It In

Before or on the due date, upload your THREE picture files (foreground, background, and merged) PLUS the python file (.py) you wrote to do the merge, to our DMS 102 section in Blackboard, in the **Project 1: Chromakey** assignment which you'll find in the Projects Turn-in area.

*Note: for this assignment, please ZIP (compress) all four files together and upload the one ZIP file to Blackboard.  (It makes it easier/faster for me to organize and grade your project.*