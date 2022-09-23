---
title: |
  Fast NTLM Cracking
description: |
  hashcat is the world's fastest and most advanced password recovery utility, supporting five unique modes of attack for over 300 highly-optimized hashing algorithms. 

  Commands:

  	hashcat64.exe -m 1000 -w 3 hash.txt ../weakpass_2a/weakpass_2a -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../weakpass_2a/weakpass_2a -r rules/d3ad0ne.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../weakpass_2a/weakpass_2a -r rules/best64.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../weakpass_2a/weakpass_2a -r rules/dive.rule -O masks/8char-1l-1u-1d-1s-compliant.hcmask


  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?d?d -O -d 3,4,5,6,7

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?d?d -O -d 3,4,5,6,7

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?d?d -O -d 3,4,5,6,7

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?l?d?d -O -d 3,4,5,6,7


  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -r rules/d3ad0ne.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -r rules/best64.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -r rules/dive.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -r rules/generated2.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -r rules/rockyou-30000.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -r rules/Incisive-leetspeak.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -r rules/T0XlCv1.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -r rules/generated.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -r rules/T0XlC-insert_00-99_1950-2050_toprules_0_F.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt ../Dutch.dic/Dutch.dic -r rules/InsidePro-HashManager.rule -O


  	hashcat64.exe -m 1000 -w 3 --session vol3 -a 3 hash.txt -i --increment-min=8 -O masks/rockyou-1-60.hcmask

  	hashcat64.exe -m 1000 -w 3 --session vol3 -a 3 hash.txt -i --increment-min=8 -O masks/rockyou-2-1800.hcmask


  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -O

  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -r rules/d3ad0ne.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -r rules/best64.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -r rules/generated2.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -r rules/dive.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -r rules/rockyou-30000.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -r rules/Incisive-leetspeak.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -r rules/T0XlCv1.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -r rules/generated.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -r rules/T0XlC-insert_00-99_1950-2050_toprules_0_F.rule -O

  	hashcat64.exe -m 1000 -w 3 hash.txt rockyou.txt -r rules/InsidePro-HashManager.rule -O

command: |
  See commands.
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
