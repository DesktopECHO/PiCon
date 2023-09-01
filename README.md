# PiCon.app
- '**_Appified_**' container runs a Linux virtual machine using the [hypervisor framework](https://developer.apple.com/documentation/hypervisor) built into macOS.  No additional software is required (Docker, VMware Fusion, VirtualBox, etc...)
- Deploys a standard Deban 12 cloud image and installs Pi-hole + Unbound with minimal user input.

## Info
 - **Intel** and **Apple Silicon** are both natively supported.  Works on any Mac built after 2010.
 - Requires macOS 10.13 or newer, bridged networking requires macOS 10.15 or newer.
 - Container uses **1/16th** of the host Mac's RAM, up to 1GB. For example, a Mac with 4GB RAM will create a 256MB virtual machine.
 - Pi-hole is persistent and starts automaticaly with your Mac using a system LaunchDaemon.  
 - [PiBar](https://github.com/amiantos/pibar) is configured during installation and appears in your menu bar at login.
 - Useful for mobile users "on the go" or as an ad-blocking DNS server for an entire network.
   
## Install
If you have an older version of PiCon installed, reset it first by holding down **Option [ ⌥ ]** while opening the app.  
 - [Download](https://github.com/DesktopECHO/PiCon/archive/refs/heads/main.zip) PiCon to your Mac.
 - Double-click the zip archive to extract its contents (Some browsers will extract the archive automatically).
 - Move `PiCon.app` to your `/Applications` folder.  This step is **_mandatory_** as the app expects to be in this location to run.
   
The first time the app is opened you will need to acknowledge a warning by Gatekeeper.  The app is digitally signed to protect against tampering but not notarized by Apple.  You can verify the signature by running `codesign -dv /Applications/PiCon.app`

## Install Screenshots
  - First-run setup:
![image](https://github.com/DesktopECHO/PiCon/assets/33142753/66fd0544-c761-41af-8eb6-22117db0d633)
  - Wait a few moments for the container to initialize.  When complete, the install summary will appear.  
  - Your web browser will open the Pi-hole admin page.  Paste your clipboard into the Pi-hole password field.
![image](https://github.com/DesktopECHO/PiCon/assets/33142753/c6d32593-6b54-42e7-98fc-9806b043293d)
 
## Post-Install Screenshots
  - PiBar is configured automatically and set to run at login.
    
![image](https://github.com/DesktopECHO/PiCon/assets/33142753/721fa0e0-7b95-480f-9cdb-abff6a035610)
  - Launch PiCon.app if you need to access the container's console.
![image](https://github.com/DesktopECHO/PiCon/assets/33142753/f0c4e5fd-24f2-4c00-aa84-b7c9e496ec37)
  - Hold down [Shift] while launching PiCon.app to restart the container.
  - Hold down Option [ ⌥ ] to reset the container and start fresh.  
![image](https://github.com/DesktopECHO/PiCon/assets/33142753/13d6fdbe-a559-4b7b-88bd-68e94cd08da4)


