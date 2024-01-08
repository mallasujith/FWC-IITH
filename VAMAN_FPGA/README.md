This contains steps to install fpga and run successfully
Steps to follow:
1) Install the zip provided i.e **fpga.zip** onto **Desktop**
2) now open terminal and go to the fpga folder
3) In here **/Desktop/fpga** type: **chmod +x setup.sh** --> This command is particularly useful for making scripts and programs executable. In this way, users can run them without typing their full path or using a dot slash (./) before their name. 
4) After this type: **sudo bash setup.sh** --> This command runs the setup file i.e installs all the required packages and modules
5) Next:
   At Home:
   sudo apt update -y
   sudo apt upgrade -y
   sudo apt install openssh-server sshpass build-essential libssl-dev libffi-dev python3-dev bison flex git tcl-dev tcl tcl-tclreadline libreadline-dev  autoconf libtool make automake texinfo pkg-          config libusb-1.0-0 libusb-1.0-0-dev gcc-arm-none-eabi libnewlib-arm-none-eabi telnet python3 apt-utils libxslt-dev cmake curl python3-pip python3-venv -y
   pip3 install gdown lxml simplejson
   sudo apt install openssh-server sshpass
   sudo apt install build-essential libssl-dev libffi-dev python3-dev bison flex git tcl-dev tcl tcl-tclreadline libreadline-dev  autoconf libtool make automake texinfo pkg-config libusb-1.0-0 libusb-1.0-0-dev gcc-arm-none-eabi libnewlib-arm-none-eabi telnet python3 apt-utils libxslt-dev python3-lxml python3-simplejson cmake curl  python3-setuptools python3-pip
   cp arch.tar.gz /home/nikhil/Desktop/fpga/arch.tar.gz
   tar -C $INSTALL_DIR  -xvf /home/nikhil/Desktop/fpga/arch.tar.gz
   export PATH="$INSTALL_DIR/quicklogic-arch-defs/bin:$INSTALL_DIR/quicklogic-arch-defs/bin/python3:$PATH"
   cd /home/nikhil/Desktop/fpga/pygmy-dev/tools/quicklogic-fasm
   nvim requirements.txt
   python3 -m venv venv
   souce venv/bin/activate
   source venv/bin/activate
   pip3 install -r requirements.txt
   sudo python3 setup.py install
   cd /home/nikhil/Desktop/fpga/pygmy-dev/tools/quicklogic-yosys
   make config-gcc
   make -j4 install PREFIX=$INSTALL_DIR
   cd /home/nikhil/Desktop/fpga/pygmy-dev/tools/yosys-symbiflow-plugins
   export PATH=$INSTALL_DIR/bin:$PATH
   make -j4 install
   cd /home/nikhil/Desktop/fpga/pygmy-dev/tools/vtr-verilog-to-routing
   make -j4
   nvim ~/.bashrc
   source ~/.bashrc
   vpr -h
   yosys -h
   qlfasm -h
   ql_symbiflow -h
   cd $INSTALL_DIR/quicklogic-arch-defs/tests/counter_16bit
   ls
   ql_symbiflow -compile -d ql-eos-s3 -P pd64 -v counter_16bit.v -t top -p chandalar.pcf -dump binary
   pip3 install gdown lxml simplejson
   ql_symbiflow -compile -d ql-eos-s3 -P pd64 -v counter_16bit.v -t top -p chandalar.pcf -dump binary
   ls
   cd /home/nikhil/Desktop/fpga
   ls
   mkdir fpga-examples
   cd fpga-examples
   svn co https://github.com/gadepall/vaman/trunk/fpga/setup/codes/blink
   cd blink
   ls
   ql_symbiflow -compile -src /home/nikhil/Desktop/fpga/fpga-examples/blink -d ql-eos-s3 -P PU64 -v helloworldfpga.v -t helloworldfpga -p quickfeather.pcf -dump binary
   ls
   nvim helloworldfpga.v
   nvim quickfeather.pcf
   ql_symbiflow -compile -src /home/nikhil/Desktop/fpga/fpga-examples/blink -d ql-eos-s3 -P PU64 -v helloworldfpga.v -t helloworldfpga -p quickfeather.pcf -dump binary
