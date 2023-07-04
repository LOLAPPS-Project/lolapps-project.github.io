---
Name: VS Code
Description: Visual Studio Code, also commonly referred to as VS Code, is a source-code editor made by Microsoft with the Electron Framework, for Windows, Linux and macOS.
Author: 'Adam Brass and Martin Sohn Christensen'
Created: 2023-01-29
Usage:
  - Steps: Override/Create a workspace/settings.json config. Add a new terminal profile with the payload in the "path" and "args" parameters. Set the new terminal profile as default.
    Description: Steps to create a VS Code terminal persitence profile
    Usecase: Establishing persistence on a Windows host
    Category: Persistence
    Privileges: User
    Limitations: None
    MitreID: T1546
  - Steps: 'Create/Modify a task in a .code-workspace file, or a tasks.json file inside a .vscode folder. Add a new task with the payload in the "command" or "args" parameters. Add one of the possible triggers: "runOption" parameter with value of "folderOpen"; or shortcut keys in the keybindings.json file.'
    Description: Steps to create and enable a VS Code task for persitence
    Usecase: Establishing persistence on a Windows host
    Category: Persistence
    Privileges: User
    Limitations: None
    MitreID: T1546
Resources:
  - Link: https://twitter.com/nas_bench/status/1618021838407495681
  - Link: https://twitter.com/nas_bench/status/1618021415852335105
  - Link: https://twitter.com/Cyb3rSn0rlax/status/1618201140008734721
Acknowledgement:
  - Person: 'Nasreddine Bencherchali'
    Handle: '@nas_bench'
  - Person: 'HAMZA'
    Handle: '@Cyb3rSn0rlax'
---
