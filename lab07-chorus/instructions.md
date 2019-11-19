Lab 7: Chorus
====================

*Due: Tuesday, November 19, 2019 (today, by 3:15 PM)*

For this in-class lab exercise, you need to cobble together several programs to achieve one goal: play a string of sounds that play a scale and then a chorus of sounds.  

Note: this lab is timed - due by the end of this class period (3:15 PM).  Labs turned-in late but before 9:00 PM that time will lose 10 points.  Labs turned-in later than that will lose 20 points.

## Requirements

- [ ] Create a file called **lab07.py** in which you'll write the program and a test case to run it.

For this lab, you'll need to re-use several previously written programs (from the book), some of which you may need to edit/tweak a little bit to work correctly with this assignment.  In addition to the programs from the book...

- [ ] Create a function named **tones()** which accepts one sound object as parameter.  Note: this function will *not* need to return anything.  All output can be done from within this function.

| Algorithm                                                    | Explanation (hints)                                          |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Start with a sound object of you singing a single note for about a second. | Record yourself saying "ahh" then save the sound as a WAV file.  Use a 22,100 sampling rate to simplify things later on. (Use a site like this which allows you to specify the sampling rate: [online-convert.com](https://audio.online-convert.com/convert-to-wav))<br><br>Then in JES, turn the WAV file into a sound object. |
| Clip the sound so there is no silence at the beginning or end of the sound. | Load the sound object in the Explore application and figure out a good place to "clip" the sound, i.e. the start and end sample numbers.<br><br>Then run the sound object through the `clip()` program (Program 105) |
| Change the sound four times, starting with the normal sound, then each time going up in pitch by a quarter, then by half, then by double. | Use the `shift()` program (Program 119) four times to create four different sound objects using factors of `1.0` then `1.25` then `1.5` then `2.0` |
| For each of those four sounds, reduce their volume by half to make sure there's no clipping when the sounds are blended with each other. | Use the `decreaseVolume()` program (Program 94) four times to reduce each sound file by half |
| Then make a fifth sound created by blending the four sounds into one, and then normalize it. | Use `addSounds()` (Program 122) and edit it to accept four sound files instead of two.  Run the four previously created sound files through that program to create the blended sound |
| Finally, play all five sounds, one after another and then display the sound in the Explore application. | Use the `blockingPlay()` function of JES to play each of the five sounds, one after another, and then "Explore" the blended sound |

### Turn-in the Assignment for Credit

- When your program is working correctly, ZIP (compress) your program file and the WAV file you used
- Go into our DMS 102 section in Blackboard; in the "Lab Assignments" area find **Lab 7: Chorus**
- Upload your ZIP file to the Lab 7 assignment









