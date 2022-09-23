---
title: |
  Cracking with masks (feasible for 8-11 characters)
description: |
  hashcat is the world's fastest and most advanced password recovery utility, supporting five unique modes of attack for over 300 highly-optimized hashing algorithms. 

  Commands for 8 chars (with special char, example Utrecht01!):

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?d?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?d?d?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?d?d?d?d?s -O

  Commands for 9 chars (with special char, example Utrecht01!):

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?d?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?d?d?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?d?d?d?d?s -O

  Commands for 10 chars (with special char, example Utrecht01!):

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?l?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?d?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?d?d?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?d?d?d?d?s -O

  Commands for 11 chars (with special char, example Utrecht01!):

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?l?l?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?l?d?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?d?d?d?s -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?d?d?d?d?s -O

  Commands for 8 chars (without special char, example Utrecht2019):

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?d?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?d?d?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?d?d?d?d -O

  Commands for 9 chars (without special char, example Utrecht2019):

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?l?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?d?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?d?d?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?d?d?d?d -O

  Commands for 10 chars (without special char, example Utrecht2019):

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?l?l?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?l?d?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?d?d?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?d?d?d?d -O

  Commands for 11 chars (without special char, example Utrecht2019):

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?l?l?l?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?l?l?d?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?l?d?d?d -O

  	hashcat64.exe -m 1000 -a 3 -w 4 --session vol1 hash.txt ?u?l?l?l?l?l?l?d?d?d?d -O

  Mask Password Cracking (Example: Januari2018!):

  	hashcat64.exe -m 1000 -w 3 -a 3 hashes/DC_Pwdump_hashes.txt -O ?u?l?l?l?d?d?d?d?s

  Using multiple masks that pass the password policy:

  	hashcat64.exe -m 1000 -w 3 -a 3 hashes/DC_Pwdump_hashes.txt -O ?u?l?l?l?d?d?d?d?s masks/8char-1l-1u-1d-1s-compliant.hcmask

  Other commands:

  	hashcat64.exe -m 1000 -a 3 -w 3 -O hashes/DC_Pwdump_hashes.txt -1 ?l?d ?1?1?1?1?1?1?1?1?1 -i --increment-min=5

  	hashcat64.exe -a 0 -m 1000 -w 3 hashes/DC_Pwdump_hashes.txt wordlist/10_million_password_list_top_1000000.txt -r rules/best64.rule -O

  	hashcat64.exe -a 0 -m 1000 -w 3 hashes/DC_Pwdump_hashes.txt wordlist/weakpass_2a -O -r rules/best64.rule

  	hashcat64.exe -m 1000 -w 3 hashes/DC_Pwdump_hashes.txt wordlist/HashesOrg -O -r rules/d3ad0ne.rule

  	hashcat64.exe -m 1000 -w 3 hashes/DC_Pwdump_hashes.txt wordlist/words.dutch -O -r rules/dive.rule

  	hashcat64.exe -m 1000 -a 3 -w 4 --session wdk2 hashes/DC_Pwdump_hashes.txt ?u?l?l?l?l?l?l?l?d?d -O -d 3,4,5,6,7

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
  - https://blog.netspi.com/netspis-top-password-masks-for-2015/
---
