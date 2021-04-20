# Entry to NS3 simulation

The initial experience of the network simulation tool with the method of installation and operation. This was an additional project of the mobile and wireless networks course in the Computer Engineering Department at Taibah University. Supervised by Dr. Salah M. Abdel-Mageid


# Collaborators

[Ahmed Ibrahim Elegl](https://github.com/Ahmedie98) 

[Thamer Saleh Al-Mutairi](https://github.com/thamer122)

[Mohammad Yaser Ammar](https://github.com/MohammadYAmmar)


## Download and installation steps

OS Used: Ubuntu 16.04.4  
NS3 version: NS3 version 3.25

1- Download Ubuntu 16.04.4 from [link](http://old-releases.ubuntu.com/releases/16.04.4/)

> ubuntu-16.04-desktop-amd64.iso

2 - Download Oracle VM VirtualBox from [link](https://www.virtualbox.org/wiki/Downloads)

3 - Install Oracle VM VirtualBox 

4 - Install Ubuntu 16.04.4  in VirtualBox
> If the system options do not appear to you with 64 bit architecture, you must activate Virtualization from the BIOS

5 - From Ubuntu: Download the ns3 tool version 3.25 from [link](https://www.nsnam.org/releases/ns-3-25/download/)

6  - Move the file to Desktop or any plase you want, then click on right press in mouse to option [ open in Terminal ]

7 - Extract the file by command

    tar jxvf ns-allione-3.25.tar.bz2
    
8 - Open the folder and bulid  the tool

      cd ns-allinone-3.27/
    
     ./build.py --enable-examples --enable-tests
     
   Congratulations 🎉! The tool has been installed after waiting for the installation ⏰
   
   
## Hello simulator

To make sure the tool works, it is possible to try the simple example, but this time it is not Hello world, but Hello simulator 😎

    cd ns-3.25/
    
    ./waf --run hello-simulator

This will print the hello Simulator which indicates that ns3 is installed successfully.

You are ready to understand how to run examples! ✨

## Running examples included with the tool

The team has made an illustration of the scientific one as follows:


Whereas, the files, whether in the C ++ language or Python in order to play them, must be copied to the Scratch folder at the beginning!

After that, to run in a graphical manner, write the command as follows

    ./waf --run scratch/[program]  --vis

We will continue the rest after the discussion today 🔜
