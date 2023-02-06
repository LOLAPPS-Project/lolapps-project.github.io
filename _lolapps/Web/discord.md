---
Name: Discord
Description: Discord is a VoIP and instant messaging social platform.
Author: 'John Jackson'
Created: 2023-01-14
Usage:
  - Steps: Create a new discord account. Login and click on the plus sign that says Add a Server on the left hand side. Create a new server, ensure that its public. In the general channel, click on the plus symbol on the message bar and click upload. Fire up Burpsuite and turn proxy intercept mode on, click on the attachment to intercept the request. Right click on the GET request in Burpsuite and click on copy link. Youll now have a direct link to the malware via discords CDN.
    Description: Steps to host malware
    Usecase: Hosting malware with a limited budget
    Category: Malware Hosting
    Privileges: None
    Limitations: Discord isnt always allowed on Enterprise networks and your malware is at the mercy of Discord
    MitreID: T1102
  - Steps: Follow the instructions per additional tooling provided in references. If you use DiscordGo, you'll have to compile your agent and configure your automation, in addition to making a server, setting up a bot, and configuring the tokens, permissions, and channels.
    Description: Steps to setup the C2 channel
    Usecase: Implant management via non-standard C2 platform
    Category: C2 Channel
    Privileges: None
    Limitations: Must rely on additional tooling
    MitreID: T1041
Resources:
  - Link: https://usa.kaspersky.com/blog/malware-in-discord/25662/
  - Link: https://unit42.paloaltonetworks.com/ukraine-targeted-outsteel-saintbot/
Acknowledgement:
  - Person: John Jackson
    Handle: '@johnjhacking'
---
