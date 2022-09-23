---
title: |
  Bruteforcing NTLM (3-8 chars)
description: |
  hashcat is the world's fastest and most advanced password recovery utility, supporting five unique modes of attack for over 300 highly-optimized hashing algorithms. 

command: |
  hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt -i --increment-min 3 --increment-max 8 ?a?a?a?a?a?a?a?a -O
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
