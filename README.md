# About VirtualBox
[ORACLE VirtualBox](https://www.virtualbox.org/) is cross-platform virtualization software that allows users to run guest operating systems inside a host operating system without having to reboot. 

Please refer to the  [user manual](https://www.virtualbox.org/manual/ch01.html)  for thoroughly information.

# About Portable-VirtualBox
Portable-VirtualBox is a free and open source software tool that lets you run [VirtualBox](https://www.virtualbox.org/) from a USB stick (almost) without separate installation. Services are started along with the tool and are removed after stopping all machines and closing the tool itself.

Initially the tool was developed and maintained by Runar Buvik. Check out his site at http://www.vbox.me/. 

# Motivation
Sometimes it can be quite handy to run VirtualBox as a portable application, because you can bundle everything together in one folder. 

In addition, switching from Hyper-V to VirtualBox and vice versa is less prolematic, if using a portable installation. Use the following command to de-/activate Hyper-V:

- `C:\Windows\System32\bcdedit.exe /set hypervisorlaunchtype off` and 
- `C:\Windows\System32\bcdedit.exe /set hypervisorlaunchtype auto`
- 
A reboot afterwards is required. This may also be of interest, if Docker for Windows is installed.

# Building

First get a copy of [AutoIt](https://www.autoitscript.com/site/) from the download section and install or extract the package. Afterwards clone this project and convert `Portable-VirtualBox.au3` with `Aut2exe_x64.exe` or `Aut2exe.exe`. 

# Running

Running VirtualBox requires the Microsofdt C++ Redistributable package. On first start of Portable-VirtualBox the tool asks for the preferred language and package extraction parameters.
On second start the tool sets up folders and settings for subsequent runs. Restart VirtualBox and Portable-VirtualBox to use this setup from now on.
