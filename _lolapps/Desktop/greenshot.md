---
Name: Greenshot
Description: Greenshot is a free and open-source screenshot program for Microsoft Windows.
Author: 'Adam Brass and Martin Sohn Christensen'
Created: 2023-01-29
Usage:
  - Steps: Any Greenshot plugin can contain persistence, the simplest being the "External command plugin" which uses command line; Modify the "Greenshot.ini" file in "%AppData%\Greenshot\", add an "[ExternalCommand]" configuration, add a new name to the "Commands" parameter, add the payload in the "Commandline.<name>" and "Argument.<name>", add the name to the "Destinations" parameter.  Alternatively, from GUI, open "Preferences -> Plugins -> External command Plugin -> Configure", add the payload in the "Command" and "Argument" parameters, open "Preferences -> Destination" and enable the new external command.
    Description: Steps to create a Greenshot plugin for persistence
    Usecase: Establishing persistence on a Windows host
    Category: Persistence
    Privileges: User
    Limitations: If using the "External command plugin" then the "Open with external command plug-in" must be installed (default). If creating/modifying a plugin then the Greenshot plugin folder (e.g. "C:\Program Files\Greenshot\Plugins") must be writeable.
    MitreID: T1546
Resources:
  - Link: https://twitter.com/martinsohndk/status/1648763069852442642
Acknowledgement:
  - Person: 'Martin Sohn Christensen'
    Handle: '@martinsohndk'
---
