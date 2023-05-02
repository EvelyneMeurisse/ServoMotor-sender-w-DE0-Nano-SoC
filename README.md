# ServoMotor-sender-with-DE0-Nano-SoC

TEAM members : MEURISSE Evelyne, DELPIRE Boris & FACCHIN Florian

----------------------

This project was realized as part of our course of Hardware/software Platforms of the master in Electrical Engineering at the Polytechnic Faculty of Mons. 

This repository contains all our personnal documents, a tutorial of our project as well as a README file to offer everyone the opportunity to understand our work and to reproduce by itself this.

The purpose of our Project is to send information to a ServoMoter using the DE0-Nano-SoC development kit. 
The useful information that we will send to the servomotor is the counter and the freqeuncy generator. This elements are details in the document "ServoMotor : Theoritical Backgrounds". This document offer the possibility to understand how a servomotor works. 

The Tuto that you can find in this repertory is divided into 2 parts : the Hardware and th Software 


HARDWARE :
----------

The hardware part of our project is the leader of the choosen input and the output. The implementation part is realized with the tool "Platform Designer" of Quartus. The programming Language used in this program in the VHDL. 
We created a program, named ServoOut, which aims to init the counter and the frequency generator.

The Hardware is also in charge to realize the Testbench, this has the purpose to simulate the behaviour of the servoOut before we link it to the Software part and the processor. It can also test the input and the output to check if the information sents to the Hardware part well-correspond to the information sents to the peripherial ( in the other to the Servomotor).

There are many VHDL codes available online to command a servomotor , it is possible to use them but the risk is that it can contain errors or need modifications to work. 

SOFTWARE : 
-----------



ADDITIONAL NOTES : PIO and GPIO - Differences and uses
------------------------------------------------------

We noticed that much people meets difficulties to understand the differences between PIO and GPIO and where it comes into our project (Hardware, Software or Peripherial ?) we realized a little resume, named "PIO and GPIO - What is that ?" if you are part of those people who are totally lost with this words.



The video that you can find at the following adress resumes all the information you need to know about our project :

--------------------------------------------------------------------------------------------------------------------------------------
Our team thanks you for the attention you pay to our work, and hopes that all this work has led you to better understand why VHDL can be used for and how to master a servo motor with a DE0-Nano-SoC kit.  
