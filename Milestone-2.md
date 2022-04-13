## Week 9 and 10 MILESTONE 2

### 

week 1 of milestone 2:  I found a spot where I could setup the webcam for my raspberry pi in my friends room that overlooks the parking lot in between the tomlinson and chidsey dorms. I tried messing around with Tensorflow for a bit, but couldn't find many helpful resources on how to implement exactly what I was looking for. I also read a couple articles that talked about how object detection might not be the most optimal way to detect cars in a parking lot. I've decided to proceed in setting up my webcam to detect if a car is in a space based on the "color of the pavement." I watched a video that went through how one could define parking spaces in a lot as objects. If I can then take what the webcam is capturing and convert the capture into what is considered a binary image I can then count the number of white pixels in the defined object spaces. If this number exceeds a preset threshold it would then be considered a non-empty space. I looked into some videos on how to make such binary image and it requires grayscaling the capture, adding a gaussian blur to it, and then using one of opencv's built in methods to convert the pixels to be either 1 or 0. The next steps for me will be setting up my raspberry pi in my friends room and then writing the code needed for what was described above.

week 2 of milestone 2: This following week I struggled to get my webcam to work with my raspberry pi consistently, along with getting my raspberry pi to display properly to my laptop. Because of this I decided to move forward with writing code that could work with my webcam. I was succesfully able to code two python scripts. The first allows me to take a still image and add rectangle objects. Using pickle I can save these objects over the image and then use the areas inside these rectangles to identify objects inside these rectangles. The next scrip overlaps the mapped out image I created from the previous script and then performs a bunch of color conversions to simplify the webcam to display a feed with pixel values represented in binary. Using the rectangles from the mapped image I can then determine the count of pixels with value 1 inside these rectangles. I so far have it setup to just display this count. The next steps for me now are figuring out how to troubleshoot my raspberry pi not displaying, creating a threshold for the pixel count inside the rectangles, adding some sort of feedback system where if the pixel count exceeds the threshold it will provide feedback, and then setting up the live feed outside my friend's window. Below are attached videos of my scripts at work: 

Image mapping using rectangles:

https://user-images.githubusercontent.com/61435118/163232798-168b6db2-fb46-4bd8-a69c-b07c492007e3.mp4

Object detecting using img filtering and thresholding:

https://user-images.githubusercontent.com/61435118/163234590-e92f9f2c-f5b3-49cb-bf2d-0c6654616ae5.mp4

