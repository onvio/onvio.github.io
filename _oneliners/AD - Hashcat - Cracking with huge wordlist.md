---
title: |
  Cracking with huge wordlist
description: |
  hashcat is the world's fastest and most advanced password recovery utility, supporting five unique modes of attack for over 300 highly-optimized hashing algorithms. 

command: |
  hashcat64.exe -a 0 -m 1000 -w 3 hashes/DC_Pwdump_hashes.txt wordlist/HashesOrg -O -r rules/best64.rule
items:
  - Hash
OS:
  - Linux
attack_types:
  - Cracking
references:
  - https://hashcat.net/hashcat/
  - https://github.com/hashcat/hashcat
---
