## WSL-CONFIG (Windows Subsystem for Linux)
  ### .wslconfig

1) Uninstall Docker

2) Enable WSL Windows 11

 ⚡ dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
 
 ⚡ dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

3) Enable the WSL for the 2


⚡wsl --set-default-version 2

4) Install Ubuntu on Microsoft Store

5) Install Windows Terminal on Microsoft Store

6) Disable the Hyper-v


 ⚡ Turn Windows features on or off


7) Create a note file .wslconfig


  %UserProfile%

  [wsl2]
  memory=8GB
  processors=4
  swap=2GB

8) Install Docker


▶️ [Install Docker Desktop on Windows](https://docs.docker.com/desktop/windows/install/) 


### Information

▶️ [Advanced settings configuration in WSL](https://docs.microsoft.com/en-us/windows/wsl/wsl-config) 


### BUG
   System.InvalidOperationException: Failed to deploy distro docker-desktop to <localpath>: exit code: -1
  
   ⚡ delete ** %USERPROFILE%/.wslconfig. **
  
  Without internet with WSL (Windows Subsystem for Linux)
  
  First option:
  
  Open Command Ubuntu:
  ⚡ sudo nano /etc/resolv.conf
  Change the na,e server value to 8.8.8.8
  nameserver xxx.xx.xx
  
  Second option:
  
  Open Command Prompt as an Administrator and type these commands:
  
  ⚡ netsh winsock reset 
  ⚡ netsh int ip reset all
  ⚡ netsh winhttp reset proxy
  ⚡ ipconfig /flushdns
  
  After reboot your machine.
  
  
  
  
