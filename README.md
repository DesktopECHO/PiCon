# PiCon.app
- _'Appified'_ container for running a Linux VM in macOS with no additional software (Docker, VMware Fusion, VirtualBox, etc...) required.
- Deploys a standard Deban 12 cloud image and installs Pi-hole with minimal user input.

## Info
 - Works on any 2010 or newer Mac.  QEMU / Lima binaries included are Intel and Apple Silicon native.
 - Requires macOS 10.13 or newer, bridged networking requires macOS 10.15 or newer
 - Container uses **1/16th** of the host Mac's RAM, up to 1GB. For example, a Mac with 4GB RAM will create a 256MB container capable of serving DNS on a typical home network.
 - Pi-hole instance is persistent across reboots and starts in the background as a system-level launch daemon.  
 - An embedded version of [PiBar](https://github.com/amiantos/pibar) is configured during installation and starts at login.
   
## Install
 - [Download](https://github.com/DesktopECHO/PiCon/releases/latest) the latest release of PiCon.app and move it to your `/Applications` folder (Note that moving the app to this location is _mandatory_)

## Install Screenshots

  - First-run setup:
![image](https://github.com/DesktopECHO/PiCon/assets/33142753/66fd0544-c761-41af-8eb6-22117db0d633)
  - Wait a few moments for the container to become ready and the installation summary will appear.
  - Your web browser will open the Pi-hole admin page.  Paste your clipboard into the Pi-hole password field.
![image](https://github.com/DesktopECHO/PiCon/assets/33142753/c6d32593-6b54-42e7-98fc-9806b043293d)
 
## Post-Install Screenshots

  - Launch PiCon.app if you need to access the container's console.
![image](https://github.com/DesktopECHO/PiCon/assets/33142753/f0c4e5fd-24f2-4c00-aa84-b7c9e496ec37)
  - Hold down [Shift] while launching PiCon.app to restart the container.
  - Hold down Option [ ⌥ ] to reset the container and start fresh.  

![image](https://github.com/DesktopECHO/PiCon/assets/33142753/13d6fdbe-a559-4b7b-88bd-68e94cd08da4)

  - PiBar is configured automatically and set to run at login.
    
![image](https://github.com/DesktopECHO/PiCon/assets/33142753/721fa0e0-7b95-480f-9cdb-abff6a035610)
