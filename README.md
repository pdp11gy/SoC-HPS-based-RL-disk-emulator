# SoC-HPS-based-RL-disk-emulator
SoC/HPS based RL01/RL02 disk emulator, Altera Cyclone V FPGA with ARM Cortex-A9 (DE10-Nano) 


**Overview**
This project is a great advancement of my RL-emulator which was based on the MAX10 FPGA,
see https://github.com/pdp11gy/DEC-RL02-RL01-disk-emulator. The architecture of the firmware 
remained the same but it had to be ported with much effort to the new SoC FPGA environment based  
on Cyclone V and Cortex-A9 processor. Originally I had used the DE0-Nano-SoC board but it was broken 
and is no longer available. I chosed the successer board DE10-Nano. This board offers many more 
possibilities and that is really great. I also use a Raspberry Pi 3 ( model B ) connected via 
network to the DE10-Nano board and use it also for development purposes with the graphical 
interface. For example: I can compile the programs like SIMH emulators and copy it to the DE10-Nano 
board, because it is binary compatible. See also https://github.com/simh/simh 

**Implementation** ( see also www.pdp11gy.com ) :
Download and unzip the file DE10_SoC_RL_emulator_V1.zip. Please read the file !README.txt.
The folder DE10_SoC_RL_emulator_V1 will include all sources and the correct setup for Quartus
Version 16.1 based on the SoC/HPS environment. The !README.txt  file also contains detailed 
instructions how to rebuild the project... or for reference purpose if you want to add another
application. 

**Summary**
This project is just the beginning. The DE10 Nano board is very flexible and still offers plenty 
of room for additional add-ons and new applications. The second PIO and the Arduino slot is still 
free and can be used for other purposes, even for non-DEC applications, maybe MFM emulator.
It would be nice if a cooperation works here.
