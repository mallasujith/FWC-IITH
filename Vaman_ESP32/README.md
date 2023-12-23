# This code is for utilizing vaman by uploading wifi code into it using the arduino.

## Steps to follow:
1) Intially, Follow all the steps as given in vaman/installation/termuxdebian/termuxubuntu_esp32.txt
2) **or** Download all the files that i provided and do the installations in <b> point3</b>
3) apt update && apt upgrade <br>
   apt install python3-pip <br>
   pip3 install platformio <br>
   pio lib --global install "stempedia/DabbleESP32" <br>
   .pio/build/esp32doit-devkit-v1/firmware.bin <br>
4) After performing the first step, a setup file will be created. or if you perform step 2 and 3 you can skip the 4th step.
5) In the setup file There will be 
