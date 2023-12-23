# This consists of files in order to upload to Vaman_PYGMY
## Steps to follow:
1) Open termux and follow installation steps from **vaman/installation/termuxdebian/termuxdebian_arm.txt**
2) open main.c to edit the code to your preferences. The file main.c is available in **/data/data/com.termux/files/home/arm-examples/blink/src/main.c**
3) After making necessary modifications, **save** your file and exit.
4) To execute and **generate bin** file: Move to path **blink/GCC_Project**
5) Type make -j4 to generate bin file.
6) **Path** for blink.bin **GCC_Project/output/bin/blink.bin**
7) Transfer the dot bin file to the pc along with the files that are included in the git.**Make sure that all the files are in the same location example :home**
8) **Update flash.sh:** sudo python3 /home/**Username**/TinyFPGA-Programmer-Application/tinyfpga-programmer-gui.py --port /dev/ttyACM0  --appfpga top.bin --m4app  blink.bin --mode m4-fpga --reset. (Replace Username with your pc's username)
9) To get the pc's username type **whoami** in terminal, After editing save the file and exit.
10) Now **connect the vaman to pc**.
11) Make sure that vaman is in **Download mode**, i.e Green Led must be blinking.
12) **To enable Download Mode**: Press **RST** button once and then press **USR** button twice, this should do the job.
13) The code gets Successfully Booted.
