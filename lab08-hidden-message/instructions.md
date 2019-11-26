Lab 8: Hidden Message
====================

*Due: Tuesday, November 26, 2019 (today, by 3:15 PM)*

For this in-class lab exercise, you need to cobble together several programs to achieve one goal: create a hidden message in a picture and share it with the class (in its hidden form).

Note: this lab is timed - due by the end of this class period (3:15 PM).  Labs turned-in late but before 9:00 PM that time will lose 10 points.  Labs turned-in later than that will lose 20 points.

## Requirements

- [ ] Create a file called **lab08.py** in which you'll write the program and a test case to run it.
  - Note: you will *not* be turning-in the lab08.py; you'll turn-in it's output only; but keep the lab08.py file for future reference

For this lab, you'll need to re-use several previously written programs (from the book)

### Create Message Image - Function

Note: this function is not in the book.

- [ ] Create a function that creates an picture with embedded text (a message that will be hidden later)

Here is the code for to create the picture (you can copy and paste this code into JES)

```python
# ******************************************
# Function to create a hidden message
# ******************************************
# Inserts a text message into a blank picture;
#   the size of the picture is based on the 
#   size of an inputted picture object
def createMsgImg(imageInput, textInput):
  canvas = makeEmptyPicture(getWidth(imageInput),getHeight(imageInput))
  addText(canvas,10,20,textInput)
  for pixel in getPixels(canvas):
    if (distance(getColor(pixel),black) < 200.0):
      setColor(pixel,black)
  return canvas
```

You need to create a TEST case for the **createMsgImg()** function:

- [ ] Set the media path (you can comment-out this line once you run it once)
- [ ] Get a picture (any) that's no more than about 800px wide and turn it into a picture object; hold it in a variable for now
  - This will be your "hider" picture into which you'll hide a text message later
  - You need the hider picture now just to get its height and width

- [ ] Prompt the user to "Enter a secret message" using the `requestString()` function; hold the inputted string in a variable for now
- [ ] Run the **createMsgImg()** function using the hider picture and the text message as arguments; capture its returned output in a variable
  - You can call the variable whatever you want so long as it makes sense for what's doing
  - You can **explore()** the variable just to check that it worked

### Encode the Message

After you get the Create Message Image function (above) to work, comment-out its TEST code.

- [ ] Use the **encode()** program (**Program 155 on page 352**) to insert your message picture (the outputted variable from the previous step) into the picture you selected as the hider
  - The encode() program should have a comment-block above it to delineate where it starts compared  to the previous code above it
- [ ] Write a test case to run the encode() program
  - Write the "original" (the hider picture) to a file using `writePictureTo()` (use a filename that makes sense for what it's doing)
  - Hold on to that file - you'll turn that in

### Test the Encoded Message

Make sure you've encoded the hidden message correctly by testing the decoding process.

After you get the Encode function (above) to work, comment-out its TEST code.

- [ ] Use the **decode()** program (**Program 156 on page 352**) to decode your message from the picture you selected as the hider
  - The decode() program should have a comment-block above it to delineate where it starts compared  to the previous code above it

- [ ] Write a test case to run the decode() program
  - Hard code your filename into the test case
  - Capture its returned output (a picture object) in a variable 
  - **explore()** the outputted picture object - make sure you can read the hidden message to confirm the encoding process (previous step) worked

NOTE: the output from the decode() program is used only to test that the encoding process worked. If it did,  do the next step...

### Publish the Encoded Message (only)

- [ ] Post the picture file with the hidden message to our DMS 102 Slack Workspace, in the #chatter channel.  

When the professor successfully decodes your message, you will get credit for this lab.  (pass/fail)

- NOTE: there's nothing for you to post in Blackboard for this lab
- Also note, the professor will post your hidden message text in Slack as a comment to your image (just keep that in mind when composing your hidden message!)









