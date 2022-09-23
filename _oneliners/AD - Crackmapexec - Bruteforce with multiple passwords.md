---
title: |
  Bruteforce with multiple passwords
description: |
  "CrackMapExec (a.k.a CME) is a post-exploitation tool that helps automate assessing the security of large Active Directory networks." - https://github.com/byt3bl33d3r/CrackMapExec/wiki. This command will bruteforce 

  Command Reference:

  	Protocol: f.e. SMB

  	Target(s): f.e. 192.168.4.0/24

  	-u: username(s) / usernames file

  	-p: password(s) / passwords file

  Command Reference:

  	crackmapexec <protocol> <target(s)> -u username1 username2 -p password1

  	crackmapexec <protocol> <target(s)> -u ~/file_containing_usernames -p ~/file_containing_passwords

  	crackmapexec <protocol> <target(s)> -u ~/file_containing_usernames -H ~/file_containing_ntlm_hashes

command: |
  crackmapexec SMB 192.168.4.0/24 -u username1 -p password1 password2
items:
  - Username
services:
  - SMB
attack_types:
  - Enumeration
OS:
  - Linux
references:
  - https://github.com/byt3bl33d3r/CrackMapExec
  - https://github.com/byt3bl33d3r/CrackMapExec/wiki
---
