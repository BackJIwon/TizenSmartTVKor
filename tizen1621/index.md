# SDK 설치하기

> This document guides how to install Tizen-based Samsung TV SDK.

---

#### 목차
 * 시스템 요구사항
 * 윈도우에서 설치하기
 * 리눅스에서 설치하기
 * CPU 가상화 지원을 위하여 확인해야 할 사항들

---

The Tizen-based Samsung TV SDK is supported on the Windows, Mac OS X, and Linux platforms. Please refer to the sections below for installation instructions for your operating system.

## 시스템 요구사항

Processor : Dual Core 1.5GHz / Single Core 3GHz or higher
RAM : at least 4GB memory (8GB recommended)
Supported CPU VT (How to check this : Checking for CPU Virtualization
Windows, and Linux OS, Mac(support soon)
Windows 7 or above. 64-bit only supported.
Windows7 32bit is not supported
Linux : This SDK has been tested on Ubuntu 12.x.
In case of Ubuntu, sudo authority

## 윈도우에서 설치하기

Download and Run the Install Manager from the Downloads page.

![](./_images/Installmanager_1(2).jpg)

Click the “Next” button.
 

Accept the license agreement and click "Next"
 

Choose a location and then click “Next”. The Tizen-based TV SDK software will install itself :
 

Waiting for installation progress complete. 
 

After the installation completes, click the “Close” button. It is also recommended that you restart your computer.
 

After the installation completes, you can find the Tizen-based TV SDK in your Start menu.

## 리눅스에서 설치하기

Download and Run the Install Manager(inst-manager.bin) from the Downloads page. 
Prerequisites (Ubuntu)
Admin Rights
Linux Administrator authority is required.
Java
Oracle Java 6 or later (Do not use Open JDK). Install with the following commands :
$ sudo add-apt-repository ppa:webupd8team/java
$ sudo apt-get update
$ sudo apt-get install oracle-java6-installer
Packages
Ubuntu requires prerequisite packages to be installed. Please execute the following commands based on your version of Ubuntu :

Ubuntu 12.04 :
$ sudo apt-get install procps gettext libdbus-1-3 libcurl3 expect grep zip make qemu-user-static libwebkitgtk-1.0-0 libudev-dev libgnome2-0 libpng12-0 libpython2.7 libpixman-1-0 ruby

Ubuntu 12.10 , 14.04 :
$ sudo apt-get install procps gettext libdbus-1-3 libcurl3 expect grep zip make qemu-user-static libwebkitgtk-1.0-0 libudev-dev libsdl1.2debian libgnome2-0 libpng12-0 libpython2.7 libpixman-1-0 ruby
 
## CPU 가상화 지원을 위하여 확인해야 할 사항들

CPU virtualization is required for the Emulator. The IDE can still be used if virtualization is not supported. Please follow the steps below to determine if your PC supports virtualization. 
Checking in Windows
If your PC is a Windows PC with an AMD CPU, then the Emulator cannot be launched. Unfortunately, AMD’s virtualization technology (AMD-v) is not supported.
If you have a Windows PC with an Intel CPU, then please visit the Intel site (http://ark.intel.com). Look for your CPU specification in the VT-x field. If the value is “yes”, then you can use the Emulator. 

 
Checking in Ubuntu
If you have a Linux Machine, then please run this command at the terminal : 
$ egrep '(vmx|svm)' /proc/cpuinfo
If you see vmx or svm at the terminal, that you can run the Emulator :

 
Virtualization Tip
Sometimes a CPU supports virtualization, but the switched is disabled in the BIOS. If you think your CPU supports virtualization,
Please check the BIOS and make sure virtualization is enabled. The following picture shows what the menu option looks like on some systems :

Remember that virtualization is only required for the Emulator. 
Follow below steps for intalling the SDK.
 

Accept the license agreement and click "Next"
 

Select “Install the new Tizen-based Samsung TV SDK version” and click the “Next” button.
 

Choose a location and then click “Next”. The Tizen-based TV SDK software will install itself :
 

Waiting for installation SDK.
 
 
After the installation completes, click the “Close” button. It is also recommended that you restart your computer.
 

After the installation completes, you can find the Tizen-based TV SDK in your Start menu.
