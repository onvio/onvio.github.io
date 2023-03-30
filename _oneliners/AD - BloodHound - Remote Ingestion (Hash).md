---
title: |
  BloodHound Remote Ingestion with Hash

description: |
  bloodhound-python is a Python based ingestor for BloodHound, based on Impacket. It allows you to remotely collect data for bloodhound by querying LDAP

  Command Reference:

  	Target IP: 10.10.10.1

  	Domain: test.local

    User: test

    Hashes: LM:NTLM / NTLM

    DC: DC01

command: |
  sudo bloodhound-python -u test -d test.local --hashes aad3b435b51404eeaad3b435b51404ee:B4B9B02E6F09A9BD760F388B67351E2B -dc DC01 -c all
items:
  - Hash
services:
  - LDAP
attack_types:
  - Enumeration
OS:
  - Linux
  - Windows
references:
  - https://github.com/BloodHoundAD/BloodHound
  - https://github.com/fox-it/BloodHound.py
---
