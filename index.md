---
layout: home
title: FPGA VGA Driver Project
tags: fpga vga verilog
categories: demo
---

For this project I chose an image that I wanted to display on the screen, for my image i chose the S from Shrek. I started by opening the colour stripes code we had gotten as a sample and adapted it to my own.
This included initializing a clock aswell.

## **Template VGA Design**
### **Project Set-Up**
I began my project by creating a new Vivado project. I included source files and a testbench given to me by my lecturer. This was really helpful to build a foundation to work off of.
For the first exercise I had to generate the clock. we did this using the ip catalog and set it to 25MHz. I will include an image of my project summary below.

<img src="docs/assets/images/project summary.png">

### **Template Code**
Our leturer gave us a template code for a colour stripes display. At first I looked at this code and had no idea what any of it meant as you would expect, but it didnt take long for me to gain an understanding.
This code included columns of an even width that displayed all different colours. I first started editing the rgb outputs to see what colours would be displayed and quickly learned that you can include more or less of the colours using the 4 bit binary code, This also meant you could mix colours to create others such as red and green to make yellow in many different shades based on how much red or green.

There was also different simulation sources such as VGA top and vga sync. VGA top included code to declare rows and columns and VGA Sync included code for the display size and refresh rate. I will include screenshots of both below.


#### **VGA Top**

<img src="docs/assets/images/VGAtop.png">

#### **VGA Sync**

<img src="docs/assets/images/VGAsync.png">

### **Simulation**
I first simulated the colour stripes to see how it was done. To simulate I saved the edited code and generated a bitstream. I connected the board to the monitor using a VGA cable and also connected the board to the PC to allow me to program it. After doing this the bitstream was generated so I would be able to open and connect to the board before programming it. Once i programmed the board the monitor displayed the colour stripes.
Once the first simulation was complete I could edit the code, save it, re-generate the bitstream and then re-program the device before seeing changes.
### **Synthesis**

Describe the synthesis and implementation processes. Consider including 1/2 useful screenshot(s). Guideline: 1/2 short paragraphs.
### **Demonstration**

## **My VGA Design Edit**
For my VGA design I decided to make the S from shrek. I chose this as I saw it as challenging but acheiveable. I found an image online and deicded to use it as a baseline to base my design around.
This image had already included a grid in it so I decided to make it 25 x 25 pixel grid as that would suit my project based on the display being 640 x 480.

<img src="docs/assets/images/shrek s online.png">

### **Code Adaptation**
The sample code we were given for the colour stripes included columns. My project needed columns. Rows were included in the VGA Top code so thankfully all I had to do was include the rows in my code.
I first played around with the colour stripes code to get a better understanding of it and how using the 4  bit binary in the rgb can make different colours. My project only included 4 colours, the white background, light green, dark green and black. I got lucky and the two greens I used were the first I tried. Once I got an understanding of the columns I added the rows and began making my project. 

It took me a while to get the hang of it but i made the 25 x 25 grid by adding 25 starting from 0:25 and 0:25  which would be the top left corner of the grid. I used if else statements to change every square I needed to in the grid and the default background was white. I will include a sample of my code to give you a visual understanding.

<img src="docs/assets/images/Code.png">

### **Simulation**
 It took longer and loner to generate the bitstream as I went on with my project as the code was growing so I would only be able to see my changes after a long period of time, this was not ideal if I made a mistake as I wouldnt realise for a while. It is important to make sure the code you are writing is correct. I will include a picture of my hardware manager while running a simulation.The simulation was important to make sure I wasnt making any mistakes with my code, running it every once in a while made it easy to see the changes being made.
<img src ="">
### **Synthesis**
Describe the synthesis & implementation outputs for your design, are there any differences to that of the original design? Guideline 1-2 short paragraphs.
### **Demonstration**
This is my finished design. I will show the pictures from lab 1 and 2 also.
## **Week1**
<img src="docs/assets/images/week 1 s.jpg">
## **Week2**
<img src="docs/assets/images/Wee2s.jpg">
## **Finished Project Week 3**
<img src="docs/assets/images/finisheds.jpg">






<img src="https://raw.githubusercontent.com/melgineer/fpga-vga-verilog/main/docs/assets/images/VGAPrjSrcs.png">
