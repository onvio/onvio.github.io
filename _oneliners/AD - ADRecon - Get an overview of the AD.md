---
title: |
  Get an overview of the AD with ADRecon
description: |
  As the name suggests ADRecon queries the LDAP server to give an overview of the AD you are working with. This only works if you have a valid domain user/machine account.

command: |
  PS C:>.\ADRecon.ps1 -DomainController <IP or FQDN> -Credential <domain\username>
items:
  - Username
  - Password
  - Shell
services:
  - LDAP
OS:
  - Windows
attack_types:
  - Enumeration
references:
  - https://github.com/sense-of-security/ADRecon
---
