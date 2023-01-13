---
Name: Dropbox
Description: File hosting service offering cloud storage and file synchronization
Author: 'John Jackson'
Created: 2023-01-10
Usage:
  - Category: Data Exfiltration
    Steps: Create a free dropbox account. Upload files that you want to exfiltrate. 
    Usecase: Exfiltrating data in a pinch
    Privileges: None
    Limitations: Its not uncommon to see organizations block file sharing services by using traffic inspection through tools like Symantec Blue Coat.
    MitreID: T1567.002
  - Category: Download
    Steps: Create a free dropbox account. Upload a password protected archive. Access Dropbox from the victim host and download/extract the archive.
    Usecase: Possibly whitelisted file downloading, depending on the organization.
    Privileges: None
    Limitations: The web application might be blocked.
    MitreID: T1102
Resources:
  - Link: https://www.volexity.com/blog/2020/11/06/oceanlotus-extending-cyber-espionage-operations-through-fake-websites/
  - Link: https://www.proofpoint.com/us/blog/threat-insight/good-bad-and-web-bug-ta416-increases-operational-tempo-against-european
Acknowledgement:
  - Person: John Jackson
    Handle: '@johnjhacking'
---    
