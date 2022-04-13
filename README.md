## Week 1
## Week 2

### Sanjay Sarma, The Internet of Things

- Summary: In the Internet of Things Sanjay details his work in MIT in developing RFIDs and their importance in devices people connect to. The article talks about how a couple decades ago Sanjay was excited for what the technological world in the future. He now has become growingly concerned with the security implementations of many of the devices people connect to today. Sanjay then highlights 3 procedures that should be a focus when implementing devices we connect to in the future
- Quote: "To leverage the power of the IoT responsibly and profitably, you need to develop and implement your own IoT technologies, solutions, and applications." This quote details one of Sanjay's concerns in how individuals should be develop their own methods of preventing security issues.
- Comment: While this article approaches the world of growing technology negatively, I believe if future devices are developed correctly they have a possibility of having beneficial lasting affects on us as humans.
- Question: Where does one draw the line on devices that encroach on our day to day lives?

## Week 3

### Julian Oliver, The Critical Engineering Manifesto

- Summary: This article goes over the basic frameworks of what it takes to become a successful critical engineer. It primarily focuses on the importance of the engineer prioritizing the user's experience when developing new technologies. It also indicates engineering as one of the most important aspects of society today. This is because it shapes the way we move communicate and think.
- Quote: "The Critical Engineer considers the exploit to be the most desirable form of exposure." I was confused with what this really meant which is why I chose to select this quote
- Comment: The way a critical engineer is supposed to think according to this manifesto sounds very similar to how one should approach testing the usability of a website.
- Question: How does one incorporate their own individuality without disrupting the user's experience with their technology?

## Week 4

### Philip K. Dick, Pay for the Printer

- Summary: This story takes place in the future where an alien species called Bitlongs has replaced the human race. The Bitlongs seem to have the ability to replicate or reproduce any item they are given. The main conflict of this story is that Bitlongs are starting to become old extinct and the humans are forced to relearn how to build. 
- Quote: "Printing means merely copying. I can't explain to you what building is; you'll have to try it yourself to find out. Building and printing are two totally different things."
- Comment: The story seemed to critique how reliant humans will be on technology in the future.
- Question: In what ways does this fictional story from 1956 reflect our reality?
## Week 5

### Brian Merchant, Everything That’s Inside Your iPhone Motherboard

- Summary: Everything that's inside your iphone is an article that highlights the raw materials that compose the iphone 6 and how those materials are collected. The main concern or issue brought up in the article is the degree of diffuclty required to obtain the materials needed to build an iphone. The article also highlights the high number of children that are emplyed in the many mines that collect these resources. The article talks about how in 2008 60 children were killed in one of the mines used to gather the iphone resources. Brian also discusses the impact this mining has had on earth, and the millions of tons that have been removed from earth.  
- Quote: "And a lot of the precious stuff is difficult to get, and mined in places with little to no regulation and dangerous, even deadly conditions."
- Comment: With how heavily dependent people are on apple's iphone I doubt many people will stop purchasing/using them even if they are aware of the harsh conditions required to build one.
- Question: How many people do you think have collectively died in order to make all apple iphones?

## Week 6

### Mayo Nissen, Unseen Sensors: Constantly Sensing but Rarely Seen

- Summary: This article has more of an optimistic approach to the world's up and coming techonological world. Instead of pointing out a lot of the negatives of technological advancements the article defends large tech companies by arguing that these companies make decisions that will benefit the general population. This article mainly talks about the large amount of sensors that go unnoticed by many specifically sensors used in public on streets or for traffic.
- Quote: "They are invisible by default. Housed in anonymous plastic or metal boxes, these sensors rarely give away even a hint as to their purpose, intention, or ownership."
- Comment: I liked that this article had a more positive approach to sensors and argued that companies make decisions to implement things to benefit the general population.
- Question: Should private companies own the data that is created in this most public of contexts?

## Week 7

### 

NO READINGS. Finalized project idea of parking sensor. Looked into flight sensor capabilities and object detection. I also looked into approach of using webcam that would require understanding openCV.

## Week 9 and 10 MILESTONE 2

### 

week 1 of milestone 2:  I found a spot where I could setup the webcam for my raspberry pi in my friends room that overlooks the parking lot in between the tomlinson and chidsey dorms. I tried messing around with Tensorflow for a bit, but couldn't find many helpful resources on how to implement exactly what I was looking for. I also read a couple articles that talked about how object detection might not be the most optimal way to detect cars in a parking lot. I've decided to proceed in setting up my webcam to detect if a car is in a space based on the "color of the pavement." I watched a video that went through how one could define parking spaces in a lot as objects. If I can then take what the webcam is capturing and convert the capture into what is considered a binary image I can then count the number of white pixels in the defined object spaces. If this number exceeds a preset threshold it would then be considered a non-empty space. I looked into some videos on how to make such binary image and it requires grayscaling the capture, adding a gaussian blur to it, and then using one of opencv's built in methods to convert the pixels to be either 1 or 0. The next steps for me will be setting up my raspberry pi in my friends room and then writing the code needed for what was described above.

week 2 of milestone 2: This following week I struggled to get my webcam to work with my raspberry pi consistently, along with getting my raspberry pi to display properly to my laptop. Because of this I decided to move forward with writing code that could work with my webcam. I was succesfully able to code two python scripts. The first allows me to take a still image and add rectangle objects. Using pickle I can save these objects over the image and then use the areas inside these rectangles to identify objects inside these rectangles. The next scrip overlaps the mapped out image I created from the previous script and then performs a bunch of color conversions to simplify the webcam to display a feed with pixel values represented in binary. Using the rectangles from the mapped image I can then determine the count of pixels with value 1 inside these rectangles. I so far have it setup to just display this count. The next steps for me now are figuring out how to troubleshoot my raspberry pi not displaying, creating a threshold for the pixel count inside the rectangles, adding some sort of feedback system where if the pixel count exceeds the threshold it will provide feedback, and then setting up the live feed outside my friend's window. Below are attached videos of my scripts at work: 

## Experiments

### Taste the power

1. -can't figure out photos
2. Multimeter acts as the eyes and ears for electrical currents
3. Quiz question: Give a step by step explanation as to how to test voltage

### Abuse a battery

1. Notes: A water analogy can be used to explain the elements of ohm's law. If you imagine a pipe that pushes water the act of pushing water through that pipe is voltage, and if you are pushing water around somewhere that can represent the current, and if that water travels through a smaller pipe that can represent resistance. The unit for voltage is volt(s), the unit for current is ampere(s), and the unit for resistance is ohm(s). AC is used for traveling longer distances like cities whereas DC can't go as far.  
2. It is more important to understand the elements of Ohm's law than the actual calculation.
3. Quiz question: What unit is used to measure current?

### Your first circuit


1. Notes: It is easier to identify a resistors resistance with a multimeter. On a circuit the voltage of a battery doesn't accumulate or add up (if you have two separate sources of power they won't add up unless you combine them)
2. Different LEDs require a different amount of power to light up. This also means different LEDs have different thresholds for how much voltage they can receive
3. Quiz question: What does each colored line represent on a resistor?
