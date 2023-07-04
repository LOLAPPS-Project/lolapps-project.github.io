---
Name: ShareX
Description: ShareX is a free and open-source screenshot and screencast program for Microsoft Windows.
Author: 'Adam Brass and Martin Sohn Christensen'
Created: 2023-01-29
Usage:
  - Steps: Locate the ApplicationConfig.json file in Documents. Create/Modify an object in the "ExternalPrograms" array. Add the payload in the "Path" and "Args" key values. Set the "IsActive" key value to "true". In the "AfterCaptureJob" key, add the value "SaveImageToFile, PerformActions". Optionally set the "HiddenWindow" key value to "true".
    Description: Steps to create a ShareX after capture task for persistence
    Usecase: Establishing persistence on a Windows host
    Category: Persistence
    Privileges: User
    Limitations: The after capture task "Save image to file" must also be enabled.
    MitreID: T1546
Resources:
  - Link: https://twitter.com/martinsohndk/status/1653445529219497987
Acknowledgement:
  - Person: 'Martin Sohn Christensen'
    Handle: '@martinsohndk'
---
