---
title: |
  Find SNMP Info
description: |
  Use nmap to scan for all hosts that are up on a network.

  Command Reference:

  	Target IP: 10.1.1.1

  	-sU: UDP Scan

command: |
  nmap -sU -p 161 -v 10.1.1.1 --script snmp*
items:
  - No_Creds
OS:
  - Linux
attack_types:
  - Scanning
references:
  - https://nmap.org/download.html
  - https://nmap.org/nsedoc/scripts/krb5-enum-users.html
---
