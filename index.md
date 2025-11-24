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
There was also different simulation sources such as VGA top and vga sync. VGA top included code to declare rows and columns and vga sync included code for the timers. I will include screenshots of both below.
### **Simulation**
Explain the simulation process. Reference any important details, include a well-selected screenshot of the simulation. Guideline: 1/2 short paragraphs.
### **Synthesis**
Describe the synthesis and implementation processes. Consider including 1/2 useful screenshot(s). Guideline: 1/2 short paragraphs.
### **Demonstration**
Perhaps add a picture of your demo. Guideline: 1/2 sentences.

## **My VGA Design Edit**
Introduce your own design idea. Consider how complex/achievabble this might be or otherwise. Reference any research you do online (use hyperlinks).
### **Code Adaptation**
Briefly show how you changed the template code to display a different image. Demonstrate your understanding. Guideline: 1-2 short paragraphs.
### **Simulation**
Show how you simulated your own design. Are there any things to note? Demonstrate your understanding. Add a screenshot. Guideline: 1-2 short paragraphs.
### **Synthesis**
Describe the synthesis & implementation outputs for your design, are there any differences to that of the original design? Guideline 1-2 short paragraphs.
### **Demonstration**
If you get your own design working on the Basys3 board, take a picture! Guideline: 1-2 sentences.

## **More Markdown Basics**
This is a paragraph. Add an empty line to start a new paragraph.

Font can be emphasised as *Italic* or **Bold**.

Code can be highlighted by using `backticks`.

Hyperlinks look like this: [GitHub Help](https://help.github.com/).

A bullet list can be rendered as follows:
- vectors
- algorithms
- iterators

Images can be added by uploading them to the repository in a /docs/assets/images folder, and then rendering using HTML via githubusercontent.com as shown in the example below.

<img src="https://raw.githubusercontent.com/melgineer/fpga-vga-verilog/main/docs/assets/images/VGAPrjSrcs.png">
