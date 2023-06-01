# ServoMotor-sender-with-DE0-Nano-SoC

TEAM members : MEURISSE Evelyne, DELPIRE Boris & FACCHIN Florian

----------------------


INTRODUCTION :
------------

This project was realized as part of our course of Hardware/software Platforms of the master in Electrical Engineering at the Polytechnic Faculty of Mons. 

This repository contains all our personnal documents, a tutorial of our project as well as a README file to offer everyone the opportunity to understand our work and to build it yourself.

The purpose of our Project is to send information to a ServoMoter using the DE0-Nano-SoC development kit. Further details are available in the document "ServoMotor : Theoritical Backgrounds". This document offers the possibility to understand how a servomotor works. 

The Tuto that you can find in this repository is divided into 2 parts : the Hardware and the Software 


HARDWARE :
----------

The Hardware part of our project is the leader of the choosen input and output.  The implementation part is achieved with the tool "Platform Designer" of Quartus. The programming Language used in this program in the VHDL. We created a program, named Servomotor, which aims to init the counter and the frequency generator. 

The Hardware is also in charge to implement the Testbench, this has the purpose to simulate the behaviour of the behaviour of the servoMotor before we link it to the Software part and the processor. It can also test the input and the output to check if the information sent to the Hardware part corresponds well to the information sent to the peripherial ( in the other to the Servomotor).

There are many VHDL codes available online to command a servomotor, it is possible to use them but the risk is that it can contain errors or need modifications to work in our case. 

In  this repository, you have a first VHDL file name "driver", this file links the hardware part (so the file "ServoMotor") to the software part. The file "wrapper" make the link between the driver and the hardware, we define here the PIO and the GPIO. 

SOFTWARE : 
-----------
The software play the role of the interface Human/Machine, it permits to enter a value of angle, and it converts it in a 8-bit value between 0 and 255. 
For this part, 2 codes in C concern this part. You will find on this repository, the files "driver.c" and "main.c". The role of the driver is to do the conversion in bits of the degree value and put in the register. The main file plays the role of the interface between the Human and the Machine.     

ADDITIONAL NOTES : PIO and GPIO - Differences and uses
------------------------------------------------------

We noticed that much people meets difficulties to understand the differences between PIO and GPIO and where it comes into our project (Hardware, Software or Peripherial ?) we realized a little resume, named "PIO and GPIO - What is that ?" if you are part of those people who are totally lost with this words.

--------------------------------------------------------------------------------------------------------------------------------------
To know how we realised the hardware and the software part, you can watch the following video (click on the link) to have more technical details about the project :

Our team thanks you for the attention you pay to our work, and hopes that all this work has led you to better understand why VHDL can be used for and how to master a servo motor with a DE0-Nano-SoC kit.  
