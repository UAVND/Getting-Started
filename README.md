# Getting-Started

A collection of documentation describing how a new member joining the team should install.

Club standards: Ubuntu 20.04 LTS, ROS Noetic
Autopilots: Ardupilot is primary used but Px4 and other autopilot systems may be used depending on the application

Robot Operating System (ROS) is a programming paradim that allows for easy communication between different computers on the same network. For the AUVSI SUAS competition ROS is used for communication between the different hardware and software systems. 

Most people either have access to a Ubuntu 20.04 LTS machine or dual boot their laptops to develop with ROS Noetic. So finding access to a ubuntu machine is the best first step . Its not too hard to dual boot your laptop, find a dual booting guide for you specific system online. (If you have a newer Mac it might be hardware locked from dual booting so check that first). If you’ve got questions about dual booting or finding a machine to work on if you can’t dual boot then let Konrad or I know and we can help.

Additonally, ubuntu can be run in a virtual machine or in the Linux for Windows program. While both of these options are functional using a virtual machine can be slow and the Linux for Windows program needs additonal system specific plugins to use functions beyond the command line. 

Dual boot links:

	Linux distro:
	https://releases.ubuntu.com/20.04/

	Dual boot guide with windows 10:
	https://linuxconfig.org/how-to-install-ubuntu-20-04-alongside-windows-10-dual-boot

	Dual booting with a Mac:
	https://www.lifewire.com/dual-boot-linux-and-mac-os-4125733

	Hardware lock on Macs info:
	Newer Macs have a thing call a T2 security chip that will stop you from booting any non-mac OS. This can be disabled but it comes with some quirks like having to boot in recovery mode all the time and the loss of some security features. 
	https://www.omgubuntu.co.uk/2018/11/apple-t2-chip-cant-boot-linux
	


Once you’ve got a ubuntu distro, working on the ROS tutorials are the next step. Install ROS Noetic with the catkin file structure. Go through the normal installation of ROS Noetic and go through the beginner tutorials until you feel you’ve got a handle on how ROS works. I found the tutorials that move an onscreen turtle around with the turtlesim package were helpful to visualize everything. 

ROS links:

	Install:
	http://wiki.ros.org/ROS/Installation

	Tutorials page:
	http://wiki.ros.org/ROS/Tutorials

	Turtlesim package:
	http://wiki.ros.org/turtlesim



Since ROS abstracts a lot of the direct hardware control moving the Turtlesim around the screen will eventually be similar to moving the whole UAV around in the sky although a lot more will be happening behind the scenes with the UAV. Everything happening behind the scenes on the UAV will be through integrating ROS with ardupilot. Ardupilot translates basic commands,like go to a specific waypoint, into the specific controls needed by the aircraft's control surfaces.

In order to interface ROS with the UAV the actual flight dynamics need to be abstracted. A flight controller and autopilot do this abstraction. We are going to be using Ardupilot for the AUVSI SUAS competition and probably for most competitions in the future. So this guild will focus on using ardupilot. Since ardupilot doesn’t have quite the same level of tutorial documentation as ROS. I think that getting an Ardupilot instance running on a simulated plane in gazebo is solid goal for getting started with Ardupilot. This should introduce you to MAVLink and a ground control software (we will most likely be using APM 2.0 but any would work fine for this).  

Ardupilot links:

	Wiki home:
	https://ardupilot.org/ardupilot/index.html

	Setting up environment on ubuntu:
	https://ardupilot.org/dev/docs/building-setup-linux.html#building-setup-linux

	Software in the Loop Simulation: Gazebo will be used for this competition 
	https://ardupilot.org/dev/docs/simulation-2.html

	ROS integration: This documentation is for both an older version of ubuntu and ros so it may not work. Konrad and I are working on getting an ardupilot + ROS example set up. Hopefully we will be done by the time you get to this part.
	https://ardupilot.org/dev/docs/ros.html


There is also a getting-started slack channel for questions related to ubuntu, dual booting, ROS, ardupilot and software in the loop (SITL) simulation. 


Additonal resources to be used for ROS, Ardupilot, and SITL practice:

The following links lead to a few tutorials and projects that use software in a similar way to UAVND. Working on any of these projects might be a fun way to practice.








  
