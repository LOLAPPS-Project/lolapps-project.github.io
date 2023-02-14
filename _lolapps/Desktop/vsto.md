---
Name: Microsoft Visual Studio Tools for Office (VSTO)
Description: VSTO is functionality available in Visual Studio, which allows the user to craft a .NET Office Add-in to be shipped with an office document.
Author: 'Abhijeet Kumar'
Created: 2023-02-10
Usage:
  - Steps: Create a VTSO document (Word, Powerpoint, etc) embedded with a DLL file written in .NET and send it to any user. Once the user opens the documents and approves the "Add-In" installation, code will be executed.
    Description: Steps to exploitation using VTSO
    Usecase: Initial Access to the system
    Category: Phishing
    Privileges: User interaction/User
    Limitations: A user with valid privileges to approve Add-in installation.
    MitreID: T1204.002
  - Steps: Utilize a different VSTO payload "Add-In" and include the code for any of the persistence techniques. After successful installation, persistence will be achieved. For more information, see "VSTO-POC" in references.
    Description: Setting up persistence using VTSO
    Usecase: Persistence
    Category: Persistence
    Privileges: User interaction/User
    Limitations: A user with valid privileges to approve Add-In installation and persistence mechanisms. Additional security software installed on system can also detect and block the persistence mechanism.
    MitreID: T1137.006
Resources:
  - Link: https://www.deepinstinct.com/blog/no-macro-no-worries-vsto-being-weaponized-by-threat-actors
  - Link: https://medium.com/@airlockdigital/make-phishing-great-again-vsto-office-files-are-the-new-macro-nightmare-e09fcadef010
  - Link: https://bohops.com/2018/01/31/vsto-the-payload-installer-that-probably-defeats-your-application-whitelisting-rules/
  - Link: https://github.com/deepinstinct/VSTO-POC
Acknowledgement:
  - Person: Abhijeet Kumar
    Handle: '@0xSapereAude'
---
