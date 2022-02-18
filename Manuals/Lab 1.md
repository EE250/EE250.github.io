# 1. Setup
### 1a) Linux Virtual Machine

Install any one of the following Virtual Machine Hypervisors on your Laptop/Desktop.

1. [VMware Fusion (Provided by VMWare Academic Program)](https://viterbiit.usc.edu/services/hardware-software/vmware-academic-program/)
2. [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

Download any one of the following Ubuntu Desktop Flavours. 
1. [Ubuntu Official Download](https://ubuntu.com/download/desktop#download)
2. [Ubuntu Mate](https://ubuntu-mate.org/download/)
  - better for older machines

Setup a new virtual machine and install Ubuntu using the ISO file downloaded in previous step.

### 1b) Git and Github

If you have not, please set up a GitHub account [connected to your USC account](https://bytes.usc.edu/github-signup/).

### 1c) Text Editors 

You may want to edit your code on your Virtual Machine.

To do this, please install any one of these on your VM:
1. [VS code by Microsoft](https://code.visualstudio.com/)(recommended)
2. [Atom Editor](https://atom.io/)
3. [Sublime Text 2/3](https://www.sublimetext.com/)
4. [Micro Editor](https://micro-editor.github.io)(optional,recommended)
 
### 1d) Flashing Raspberry Pi OS

To make your Raspberry Pi work, we need to install the Raspberry Pi Operating System on your SD Card.

1. Install Etcher(recommended) from [here](https://www.balena.io/etcher/) on your host OS(Win/MacOS/etc.)
<!-- In future, if Etcher ends support, we may opt to use `sudo apt install rpi-imager` on the Ubuntu VM -->

2. Download the Legacy Raspberry Pi OS [here](https://www.raspberrypi.com/software/operating-systems/#raspberry-pi-os-legacy)

# Using Secure Shell (SSH)
### Enable SSH on the Raspberry Pi
- `ssh pi@raspberry`
- `ssh pi@raspberry.local`
- `ssh pi@AA.BB.CC.DD` where AA.BB.CC.DD is the IPv4 address of the RPi.


###### 8. DEBUGGING
- If you can't `ping raspberrypi` or `ping raspberrypi.local` or can't find the IP address of the Raspberry Pi, you may try the App `Fing` on [iOS](https://apps.apple.com/us/app/fing-network-scanner/id430921107) or [Android](https://play.google.com/store/apps/details?id=com.overlook.android.fing&hl=en_US&gl=US).


###### 9. Micro terminal editor on your Raspberry Pi

Install using the command `sudo apt install micro` OR
install by following the instructions at [Micro Editor](https://micro-editor.github.io/)

If you wish, you may install micro terminal editor on your Ubuntu VM as well. 

### Resources
- [Overcoming Command-Line |Prof. Phillip Guo Blog Link](https://pg.ucsd.edu/command-line-bullshittery.htm)
- [Understanding Git](https://hackernoon.com/understanding-git-fcffd87c15a3)
- [Git Branching Tutorial](https://learngitbranching.js.org/)

