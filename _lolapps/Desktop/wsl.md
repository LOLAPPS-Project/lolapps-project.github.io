---
Name: Windows Subsystem for Linux (WSL)
Description: WSL gives users and developers a seemless way to run Linux environments in the Windows operating system without virtual machines or dual booting.
Author: 'Joe Helle'
Created: 2023-01-29
Usage:
  - Steps: Identify WSL or WSL2 functionality on a Windows 10 or 11 endpoint. This can be achieved by running 'where wsl' in a Command Prompt. Once identified, the command 'wsl' can be ran in either a Command Prompt or PowerShell terminal to load into the default Linux environment. Locate a suitable directory and generate a reverse shell that points to a listener or other C2 server. Backing out to the regular Command Prompt/PowerShell terminal, generate an Autorun registry edit. ```reg add “HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run” -v screendoor /t REG_SZ /d '"C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exewindowstyle hidden -c wsl --exec bash /home/themayor/temp.sh"' ``` Start the reverse shell or C2 server listener and wait for the system to reboot. 
    Description: Steps to enable persistence via Windows Subsystem for Linux.
    Category: Persistence
    Privileges: User
    Limitations: System must have Windows Subsystem for Linux installed, and the current Windows user must be able to make edits to the Registry.
    MitreID: T1547.001
Resources:
  - Link: https://medium.themayor.tech/windows-persistence-using-wsl2-8f87e319ea56
Acknowledgement:
  - Person: Joe Helle
    Handle: '@joehelle'
---
