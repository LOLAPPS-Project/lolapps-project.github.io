---
Name: WinSCP
Description: WinSCP is a free and open-source SSH File Transfer Protocol, File Transfer Protocol, WebDAV, Amazon S3, and secure copy protocol (SCP) client for Microsoft Windows.
Author: 'Adam Brass and Martin Sohn Christensen'
Created: 2023-01-29
Usage:
  - Steps: WinSCP "Commands" can contain persistence and are run upon hotkeys or interaction with the WinSCP interface. The type "CustomCommands" which are command line commands, multiple CustomCommands exists by default and are stored in "HKCU:\SOFTWARE\Martin Prikryl\WinSCP 2\Configuration\CustomCommands"
    Description: Steps to create a WinSCP "CustomCommands" persistence
    Usecase: Establishing persistence on a Windows host
    Category: Persistence
    Privileges: User or Administrator
    Limitations: None
    MitreID: T1546
  - Steps: WinSCP "Commands" can contain persistence and are run upon hotkeys or interaction with the WinSCP interface. The type "Extensions" are PowerShell .ps1 files, multiple Extensions exist by default and are stored in "%LocalAppData%\Programs\WinSCP\Extensions" or "%PROGRAMFILES(X86)%\WinSCP\Extensions".
    Description: Steps to create a WinSCP "Extensions" persistence
    Usecase: Establishing persistence on a Windows host
    Category: Persistence
    Privileges: User or Administrator
    Limitations: Requires write-access to the WinSCP directory, if installed for all users in Program Files it requires administrator privileges.
    MitreID: T1546
  - Steps: WinSCP "External editor" can contain persistence and are run upon editing a remote file. Persistence is created by setting a new external editor, setting a binary as the editor, and making the editor the preferred editor. The preferred editors is stored in "HKCU\SOFTWARE\Martin Prikryl\WinSCP 2\Configuration\Interface\Editor\0".
    Description: Steps to create a WinSCP "Extensions" persistence
    Usecase: Establishing persistence on a Windows host
    Category: Persistence
    Privileges: User
    Limitations: None
    MitreID: T1546
Resources:
  - Link: https://twitter.com/martinsohndk/status/1649678130859130882
Acknowledgement:
  - Person: 'Martin Sohn Christensen'
    Handle: '@martinsohndk'
---
