# Lab 1: Saving Programs in JES

*Due: in-class on Thursday, September 5, 2019*

This assignment simply tests your understanding of using JES to write and save programs, and to make sure you can turn-in programs in Blackboard.

## Part 1A: Install/Try JES

We'll do this part in-class on Tuesday, September 3.

*Note: installing JES on your personal computer is optional but recommended for DMS 102.  If need be, you can use the version of JES installed on the University's lab computers, but if you do, don't forget to save your files on your own storage media - a thumb drive or Google Drive.*

1. JES requires you have Java installed on your computer.  To check...

   - **Windows users**, open a Command Prompt window (CMD) and enter `java -version`

   - **Mac users**, open a Terminal window and enter `java -version`

     …depending on what you see, you may have to install additional software before proceeding: 

   - **Windows users**, so long as you don't get an error message, pretty much any version of Java will work with JES.  Proceed to Step 2 to figure out which version of JES to download.

   - **Mac users**, only Java version "1.6…" will work with JES.  If you see `java version "1.6…` proceed to Step 2.  Else, if you get an error message or a message about any other version of Java, check with the professor to figure out what to do next.

2. Go to GitHub and download the appropriate package to install JES on your personal laptop: https://github.com/gatech-csl/jes/releases/tag/5.020

3. Install or extract (depending on what version you downloaded) and put the JES files in logical area on your computer's hard drive

   - Note: you can rename the JES folder to something simple, like "**JES**"
   - Suggestion: create a folder named something like "**DMS 102**" somewhere (like your computer's Desktop), and put the **JES** folder in there

4. Download the author's "media source" files ([from here](../media/mediasources.zip)) and unzip the files into a logical area on your computer's hard drive

   - Suggestion: put the **mediasources** folder in the **DMS 102** folder along with **JES**

5. Run **JES**

   - Double-click the JES icon (Windows or Mac)
     
- Test running some code in the Command Area; see the examples in Chapter 2 in the book, starting on page 35

## Part 1B: Practice Saving Programs in JES

We'll do this part together, in-class on Thursday, September 5.

*Note: for this (or any Computer Science course) you should turn-on file extensions (make them visible) in your computer's OS*

1. Create a folder named **lab01**
2. Prep an image file

   - Use one of your own pictures - any **.jpg** file with appropriate subject matter
   - Resize and resave the image so it's no larger than about 800px wide
   - Put the image file in the **lab01** folder
3. Get a sound file

   - Find a **.wav** file that would be appropriate for the image file - it needs to be short and a relatively small file size (no more than say, 250KB or so), and it has to have some relation (meaning) to the image
     - You can find usable **.wav** files in the **mediasources** folder, or...
     - Google for WAV files and find some other appropriate file that works with your image, or...
     - If you have the capabilities to create your own **.wav** file, do so. 
   - Put the sound file in the **lab01** folder
4. Create a program file named **lab01.py** and save it in the **lab01** folder

Edit the **lab01.py** file in JES as follows...
5. Add a three-line comment block (lines 1-3) to describe the program like this

```pyt
# ********************
# Program 7: Play a Sound File While Showing a Picture
# ********************
```

6. Copy program 7 as-is, from the book (page 38)
7. Below the program, create another three-line comment block like this


```pyt
# ********************
# TEST
# ********************
```

8. Below the comment block, add the following code to test the program

```pyt
setMediaPath()
playAndShow('aaa.wav', 'bungee.jpg')
```

...except, instead of **aaa.wav** and **bungee.jpg**, insert your own file names

9. Save the program file and then click the "Load Program" button

   - The` setMediaPath()` command should prompt you to navigate to your media files (in your **lab01** folder) and then immediately play and show your sound and image files.
   - If the program doesn't work, FIGURE IT OUT!  (You need to make the program work before you turn it in.)


### Turn-in the Assignment for Credit

1. When your program is working correctly, ZIP (compress) the **lab01** folder 
2. Open a web browser and navigate to our DMS 102 section in Blackboard; in the "Lab Assignments" area find "Lab 1: Saving Programs in JES"
3. Upload your **lab01.zip** file to the Lab 1 assignment

*This assignment is pass/fail*

