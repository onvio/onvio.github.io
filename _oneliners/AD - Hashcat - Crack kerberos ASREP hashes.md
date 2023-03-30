---
title: |
  Crack kerberos ASREP hashes
description: |
  hashcat is the world's fastest and most advanced password recovery utility, supporting five unique modes of attack for over 300 highly-optimized hashing algorithms. 

  Command Reference:

  	-m: hashcat mode 18200 (Kerberos ASREP)

    --force: ignore warnings
command: |
  hashcat -m 18200 -w 3 hash.txt rockyou.txt -O
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
