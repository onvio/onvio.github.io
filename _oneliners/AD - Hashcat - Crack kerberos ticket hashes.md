---
title: |
  Crack kerberos ticket hashes
description: |
  hashcat is the world's fastest and most advanced password recovery utility, supporting five unique modes of attack for over 300 highly-optimized hashing algorithms. 

  Command Reference:

  	-m: hashcat mode 13100 (Kerberos 5 TGS)

    --force: ignore warnings
command: |
  hashcat -m 13100 -w 3 hash.txt rockyou.txt --force
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
