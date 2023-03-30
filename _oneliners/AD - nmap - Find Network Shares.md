---
title: |
  Find Network Shares using nmap
description: |
  Use nmap to find network shares.

  Command Reference:

  	Network: 192.168.4.0/24

command: |
  nmap -p139,445 --script smb-enum-shares 192.168.4.0/24
items:
  - No_Creds
services:
  - SMB
OS:
  - Linux
attack_types:
  - Scanning
references:
  - https://nmap.org/download.html
  - https://nmap.org/nsedoc/scripts/krb5-enum-users.html
---
