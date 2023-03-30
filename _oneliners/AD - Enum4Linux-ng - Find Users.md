---
title: |
  Find Users with Enum4Linux-ng
description: |
  enum4linux-ng.py is a rewrite of Mark Lowe's (former Portcullis Labs now Cisco CX Security Labs) enum4linux.pl, a tool for enumerating information from Windows and Samba systems, aimed for security professionals and CTF players. The tool is mainly a wrapper around the Samba tools nmblookup, net, rpcclient and smbclient.

  Command Reference:

  	Target IP: 10.10.10.1

command: |
  enum4linux-ng -U 10.10.10.1 | grep 'user:'
items:
  - No-Creds
attack_types:
  - Enumeration
OS:
  - Linux
references:
  - https://github.com/cddmp/enum4linux-ng
---
