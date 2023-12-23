This code is for utilizing vaman by uploading wifi code into it using the arduino.

Steps to follow:
1) Intially, Follow all the steps as given in vaman/installation/termuxdebian/termuxubuntu_esp32.txt
2) or
3) apt update && apt upgrade
   apt install python3-pip
   pip3 install platformio
   pio lib --global install "stempedia/DabbleESP32"
   .pio/build/esp32doit-devkit-v1/firmware.bin 
3) After performing the first step, a setup file will be created.
4) In the setup file There will be 
