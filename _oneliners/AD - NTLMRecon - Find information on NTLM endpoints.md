---
title: |
  Enumerate information from NTLM authentication enabled web endpoints
description: |
  NTLMRecon looks for NTLM enabled web endpoints, sends a fake authentication request and enumerates the following information from the NTLMSSP response:

  - AD Domain Name
  - Server name
  - DNS Domain Name
  - FQDN
  - Parent DNS Domain

command: |
  ntlmrecon --input https://mail.contoso.com --outfile ntlmrecon.csv
  
  ntlmrecon --input 192.168.1.1/24 --outfile ntlmrecon-ranges.csv
items:
  - No_Creds
services:
  - NTLM
OS:
  - Linux
attack_types:
  - Enumeration
references:
  - https://github.com/pwnfoo/NTLMRecon
---
