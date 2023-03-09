# Enhance!  picoCTF

## Problem

> Download this image file and find the flag >>> https://artifacts.picoctf.net/c/137/drawing.flag.svg 
  
## Hints

*There are no hints for this problem*

## Research

After downloading the file the first thing I noticed was that is was a .svg file. A quick google search told me this stood for Scalable Vector Graphics. These files are diffrent from png, jpeg, etc. because they render based on a mathmatical formula and not the number of pixels. Meaning you can zoom in and out without losing quality. 

This information combined with the problem being called *"Enhance!"* told me that I would need to either zoom in really far or zoom out really far to find the flag. 

## Approach

1. Opening the file in a browser (I used chrome) displays a black circle with a while hole in the middle. Naturally I tried to zoom into the middle of the picture. I used "Ctrl","+" along with pinching to zoom on my trackpad to zoom in. I could barely make out another black dot in the middle but I definetly could not see the flag. 

2. My next instinct was to open the file with notepad. Opening the file with notepad displayed a xml file containg the svg data. This data showed the flag in plain text! 

> <img width="517" alt="Screenshot 2023-03-09 144122" src="https://user-images.githubusercontent.com/77343317/224152820-ec80235a-07c0-422b-9910-c8f2560e8b36.png">

3. You can also do F12 on the page in you browser to see this information as well. Maybe this is a bit of an oversight, I assume this is not the intended way to solve this problem. You can probably find the flag by opening this file in photoshop as well. 


## Flag

picoCTF{3nh4nc3d_24374675}
