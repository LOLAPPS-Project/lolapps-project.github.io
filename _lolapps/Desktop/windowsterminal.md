---
Name: Windows Terminal
Description: The Windows Terminal is a terminal application developed for Windows 10 for users of command-line tools and shells like Command Prompt, PowerShell, and WSL.
Author: 'Adam Brass and Martin Sohn Christensen'
Created: 2023-01-29
Usage:
  - Steps: 'Locate the settings.json in "%LocalAppData%\Packages\Microsoft.WindowsTerminal_*\LocalState\". Add a custom profile with the payload in the "commandLine" parameter. Add the custom profile GUID to the "defaultProfile" value. Add the value "startOnUserLogin": true'
    Description: Steps to create a Terminal profile for persistence
    Usecase: Establishing persistence on a Windows host
    Category: Persistence
    Privileges: User
    Limitations: None
    MitreID: T1546
Resources:
  - Link: https://nasbench.medium.com/persistence-using-windows-terminal-profiles-5035d3fc86fe
  - Link: https://infosecwriteups.com/stealthy-persistence-while-using-windows-terminal-ff6f4927563a
Acknowledgement:
  - Person: 'Nasreddine Bencherchali'
    Handle: '@nas_bench'
  - Person: 'bob van der staak'
    Handle: '@securityBeserk'
---
