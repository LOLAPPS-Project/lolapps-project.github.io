---
Name: Zix Secure Messaging
Description: Enterprise tool to compose, receive, view, reply to, and forward encrypted messages over the internet.
Author: 'John Jackson'
Created: 2023-01-09
Usage:
  - Steps: Attempt to locate the zix secure messaging portal for the organization and check to see if you have the ability to register an account. Register an account with a custom email that looks like it could actually belong to an employee. Zip any files you want to exfiltrate from the workstation. Compose a new message, and address it to an employee that doesnt actually exist in the system. You can now retrieve the files on a different device by logging in and viewing the sent mail tab.
    Description: Steps to exfiltrate data using day-to-day enterprise tooling
    Usecase: Exfiltrating data in heavily monitored environments
    Category: Data Exfiltration
    Privileges: None
    Limitations: Need to be able to register an account or gain access to one. Can only exfiltrate a specified amount of data per message.
    MitreID: T1567
  - Steps: Register a zix secure messaging account for the company. Upload a zip-encrypted archive with your payload in it. Compose a new message and send it to an employee that doesnt exist. Login from the victim host machine, download, unzip, and execute the payload.
    Description: Steps to setup an account and download your malware by a whitelisted solution.
    Usecase: Leveraging external tooling for proxy inspection bypass
    Category: Download
    Privileges: None
    Limitations: Need to be able to register an account or gain access to one. Can only upload a specified archive size per message.
    MitreID: T1105
  - Steps: Register a zix secure messaging account using multiple employee email addresses. Save all of the emails and passwords registered. If an employee clicks the approve button, youll now have their newly registered account to use for whitelisted phishing.
    Description: Steps to attempt phishing with tools recognized/allowed by the company
    Usecase: Whitelisted phishing since Zix will probably be allowed if the company uses it
    Category: Phishing
    Privileges: User interaction/User
    Limitations: An employee must click the account approval button. In addition, organizations can require an account creation code instead of an approval button.
    MitreID: T1566.003
Resources:
  - Link: https://johnjhacking.com/blog/zix-exfiltration/
  - Link: https://johnjhacking.com/blog/zix-spearphishing/
Acknowledgement:
  - Person: John Jackson
    Handle: '@johnjhacking'
---
