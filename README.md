# SoC/HPS-based-RL01/RL02-disk-emulator
SoC/HPS based RL01/RL02 disk emulator, Altera Cyclone V FPGA with ARM Cortex-A9 (DE10-Nano) 


The operation of the RL02/RL01 emulator is best viewed with a VIDEO via YouTube, however in the first version from **2012**, based on the DE1-Board. https://www.youtube.com/watch?v=0i3ypBU39as


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
Download and unzip the file DE10_SoC_RL_emulator_V2.zip. Please read the file !README.txt.
**The folder DE10_SoC_RL_emulator_V2_2 contains all sources** and the correct setup for Quartus                             
Version 16.1 based on the SoC/HPS environment. The !README.txt file contains detailed instructions
how to rebuild the project... or for reference purpose if you want to add another application.                                
 

**Updates**                                                                                         
Version **2.2** : Full suppert for **.DSK** image file. The rlemulator is using now also .DSK disk image 
files, which contain the raw dump of a disk. At write operation, the .DEC file and the .DSK file will be 
written. At read operation, first try is to read the .DEC file. If it does not exist,the .DSK file will 
be read. Best interface to the SIMH project. Implementation of a possibility of external Reset/Reconfig 
buttons. More details with an example in the user manual.                                                                         
**Update:** The issue "load FPGA(.rbf file) from Linux"  was solved mainly by the GitHub reference :                      
https://github.com/nhasbun/de10nano_fpga_linux_config . detailed information, see  manual Get_started.pdf.                       
                                                                                                                               
For info: Another project, MFM disk emulator, also based on the DE10-Nano board is now also available:                   
https://github.com/pdp11gy/SoC-HPS-based-MFM-disk-emulator  It is planned to bring these two projects                       
together see also overview.jpg. Details will be published on my homepage.
                                                                                                                               


