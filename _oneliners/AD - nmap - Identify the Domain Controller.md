---
title: |
  Identify the Domain Controller
description: |
  Use nmap to identify the Domain Controller.

  Command Reference:

  	Network: 10.1.1.*

command: |
  nmap -p 389,636 10.1.1.*
items:
  - No_Creds
services:
  - LDAP
OS:
  - Linux
attack_types:
  - Scanning
references:
  - https://nmap.org/download.html
  - https://nmap.org/nsedoc/scripts/krb5-enum-users.html
---
