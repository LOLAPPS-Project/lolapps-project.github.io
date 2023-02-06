---
Name: Remote Desktop Connection
Description: Software to interact using the Protocol developed by Microsoft which provides a user with a graphical interface to connect to another system over a network connection.
Author: 'John Jackson'
Created: 2023-01-13
Usage:
  - Steps: Deploy a TCP/UDP tunnel or proxy agent such as Chisel or Ligolo. Once on the internal network, connect to the first machine via xfreerdp (Linux) or Remote Desktop Connection (Windows). Open up the Windows start menu and type in Remote Desktop Connection. Click on it and enter in the IP address of a host on the network. You can now pivot to another host with valid credentials. Alternatively, something headless such as SharpRDP can be used. If RDP isnt enabled but you have credentials for a domain admin, or a user with administrative access to the target system, you can possibly use crackmapexec to enable RDP.
    Description: Steps to connect to another host
    Usecase: Compromising other hosts with valid credentials
    Category: Lateral Movement
    Privileges: User
    Limitations: The user may not have access to the host, or RDP might be disabled. The user might not be in the right access group. Internal access to the network is needed.
    MitreID: T1021.001
Resources:
  - Link: https://github.com/jpillora/chisel
  - Link: https://github.com/sysdream/ligolo
  - Link: https://github.com/0xthirteen/SharpRDP
  - Link: https://cheatsheet.haax.fr/windows-systems/exploitation/rdp_exploitation/
  - Link: https://posts.specterops.io/revisiting-remote-desktop-lateral-movement-8fb905cb46c3
  - Link: https://www.crowdstrike.com/blog/carbon-spider-embraces-big-game-hunting-part-1
Acknowledgement:
  - Person: John Jackson
    Handle: '@johnjhacking'
---
