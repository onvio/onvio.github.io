---
title: |
  Enumerate valid AD accounts through Kerberos Pre-Auth
description: |
  ropnop's kerbrute bruteforces and enumerates valid Active Directory accounts through Kerberos Pre-Authentication. The following command will attempt to enumerate valid usernames given a list of usernames to try.

  Command Reference:

  	DC IP: 10.10.10.1

  	Domain: test.local

  	Users List: usernames.txt

command: |
  kerbrute userenum --dc 10.10.10.1 -d test.local usernames.txt
items:
  - No_Creds
services:
  - Kerberos
OS:
  - Linux
  - Windows
attack_types:
  - Enumeration
references:
  - https://github.com/ropnop/kerbrute
---
