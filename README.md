## WSL-CONFIG
  ### .wslconfig

1) Uninstall Docker

2) Enable WSL Windows 11

 ⚡ dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
 
 ⚡ dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

3) Enable the WSL for the 2


⚡wsl --set-default-version 2

4) Install Ubuntu on Microsof Store

5) Install Windows Terminal

6) Disable the Hyper-v


 ⚡ Turn Windows features on or off


7) Create a note file .wslconfig


  %UserProfile%

  [wsl2]
  memory=8GB
  processors=4
  swap=2GB

8) Instalar o Docker
