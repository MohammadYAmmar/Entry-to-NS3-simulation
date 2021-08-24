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
> If the system options do not appear to you with 64-bit architecture, you must activate Virtualization from the BIOS

5 - From Ubuntu: Download and install required packages, from these commands in terminal 

      sudo apt update
    
     ./build.py --enable-examples --enable-tests

6 - From Ubuntu: Download the ns3 tool version 3.25 from [link](https://www.nsnam.org/releases/ns-3-25/download/)

7  - Move the file to Desktop or any place you want, then click on the right press in mouse to option [ open in Terminal ]

8 - Extract the file by command

    tar jxvf ns-allione-3.25.tar.bz2
    
9 - Open the folder and build  the tool

      cd ns-allinone-3.25/
    
     sudo apt-get install build-essential autoconf automake libxmu-dev python-pygoocanvas python-pygraphviz cvs mercurial bzr git cmake p7zip-full python-matplotlib python-tk python-dev python-kiwi python-gnome2 python-gnome2-desktop-dev python-rsvg qt4-dev-tools qt4-qmake qt4-qmake qt4-default gnuplot-x11 wireshark
     
 Then enter Y to confirm download
     
     > Do not worry when you do not see the password 👀 when you are typing, this is a safety measure in Linux systems 😁
     
     
   Congratulations 🎉! The tool has been installed after waiting for the installation ⏰
   
   
## Hello simulator

To make sure the tool works, it is possible to try the simple example, but this time it is not Hello world, but Hello simulator 😎

    cd ns-3.25/
    
    ./waf --run hello-simulator

This will print the hello Simulator which indicates that ns3 is installed successfully.

You are ready to understand how to run examples! ✨

## Running examples included with the tool

The team has made an illustration of the scientific one as follows:

![alt text](https://github.com/MohammadYAmmar/Entry-to-NS3-simulation/blob/main/Pictures%20and%20GIF%20using%20in%20ReadMe/GIF%20Steps%20animation%20to%20run%20examples.gif "GIF Steps animation to run examples")


Whereas, the files, whether in the C ++ language or Python in order to play them, must be copied to the Scratch folder at the beginning!

After that, to run in a graphical manner, write the command as follows

    ./waf --run scratch/[program]  --vis
    
# Examples of running example
Simulation run experience

![alt text](https://github.com/MohammadYAmmar/Entry-to-NS3-simulation/blob/main/Pictures%20and%20GIF%20using%20in%20ReadMe/GIF%20run%20wifi%20adhoc%20edit1.gif "GIF Steps to run adhoc")

We will continue the rest after the discussion today 🔜 (Actually  🔜 = After 4 months :) )

# WIFI Ad Hoc

The beginning of the mods is to increase the number of noods from 2 to 5

`NodeContainer c;
  c.Create (2); //old
  c.Create (5);`

In addition to placing places for them and assigning them to them. from 2 nodes to 5

`/*
  positionAlloc->Add (Vector (0.0, 1.0, 2.0));
  positionAlloc->Add (Vector (5.0, 6.0, 7.0));
positionAlloc->Add (Vector (3.0, 3.0, 5.0));
*/`

to

`positionAlloc->Add (Vector (0.0, 1.0, 1.0));
  positionAlloc->Add (Vector (5.0, 5.0, 5.0));
  positionAlloc->Add (Vector (10.0, 10.0, 10.0));
  positionAlloc->Add (Vector (15.0, 15.0, 15.0));
  positionAlloc->Add (Vector (20.0, 20.0, 20.0))`

The the process in GIF
   ![alt text](https://github.com/MohammadYAmmar/Entry-to-NS3-simulation/blob/main/Pictures%20and%20GIF%20using%20in%20ReadMe/GIF%20Modification%20Ad-hoc.gif "Modification in Ad-hoc")


# Performance metrics on Third

At first, this is the result of running the file without modification

During work, there was a meeting via Microsoft Times with Ahmed and Thamer :)

![alt text](https://github.com/MohammadYAmmar/Entry-to-NS3-simulation/blob/main/Pictures%20and%20GIF%20using%20in%20ReadMe/GIF%20of%20thrid.gif "GIF of thrid")


To activate the possibility of modification, we have done many options, as we note in this picture, such as increasing the time

![alt text](https://github.com/MohammadYAmmar/Entry-to-NS3-simulation/blob/main/Pictures%20and%20GIF%20using%20in%20ReadMe/Picture%201%20of%20thrid.png "Picture 1 of thrid")

Then allow the creation of a third of the new files

![alt text](https://github.com/MohammadYAmmar/Entry-to-NS3-simulation/blob/main/Pictures%20and%20GIF%20using%20in%20ReadMe/Picture%202%20of%20thrid.png "Picture 2 of thrid")


`// bool tracing = false;`

But after enable will be
 ` bool tracing = true;`




# Trace metrics
This tool was used and built-in Java
This is the tool experience for the third example of the tool

[Trace metrics](https://sourceforge.net/projects/tracemetrics/
)

The tools need to download Jave JRE by the command in terminal

`sudo apt install default-jre`

![alt text](https://github.com/MohammadYAmmar/Entry-to-NS3-simulation/blob/main/Pictures%20and%20GIF%20using%20in%20ReadMe/GIF%20Trace%20matrics.gif "GIF OF Trace metrics")


# Challenges
- It was hard to install the tool
- It was a challenge for us to start the simulation
- Other tool for performance matrices like with java

# Versions
| Versions  | Run visual simulate by group |
| ------------- | ------------- |
| 3.33  | ❎  |
| 3.31  | ❎  |
| 3.29  | ❎  |
| 3.27  | ❎  |
| 3.25  | ✅  |

Because of that, I'm thinking of doing a shell script to install the version with simple steps soon, God willing 🔜

A picture during the installation of the tool in the Thamer device

![alt text]( "A picture of the installation by Thamer")




