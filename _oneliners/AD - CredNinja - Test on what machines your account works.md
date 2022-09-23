---
title: |
  Test on what machines your account works
description: |
  A multithreaded tool designed to identify if credentials are valid, invalid, or local admin valid credentials within a network at-scale via SMB, plus now with a user hunter

  Command Reference:

  	users.txt = accounts list DOMAIN\user:password

  	hosts.txt = target IP list

command: |
  python3 CredNinja.py -a users.txt -s hosts.txt
items:
  - Username
  - Password
services:
  - SMB
OS:
  - Linux
attack_types:
  - Enumeration
references:
  - https://github.com/Raikia/CredNinja
---
