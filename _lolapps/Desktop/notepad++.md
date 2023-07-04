---
Name: Notepad++
Description: Notepad++ is a free source code editor and Notepad replacement that supports several languages.
Author: 'Adam Brass and Martin Sohn Christensen'
Created: 2023-01-29
Usage:
  - Steps: Compile code and generate a DLL plugin file. Create a custom plugin folder in the plugins directory, for example "C:\Program Files\Notepad++\plugins\" and place the DLL plugin file in the directory. The directory and DLL must have the same name.
    Description: Steps to create and enable a Notepad++ persistence plugin
    Usecase: Establishing persistence on a Windows host
    Category: Persistence
    Privileges: Administrator
    Limitations: Requires administrative privileges if Notepad++ is installed within %PROGRAMFILES% (default directory) or any other administrative write-protected directory.
    MitreID: T1546
Resources:
  - Link: https://offensivedefence.co.uk/posts/notepad++/
  - Link: https://pentestlab.blog/2022/02/14/persistence-notepad-plugins/
Acknowledgement:
  - Person: 'Rasta Mouse'
    Handle: '@_RastaMouse'
  - Person: 'netbiosX'
    Handle: '@netbiosX'
---
