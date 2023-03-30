---
title: |
  Dump Active Directory Information with LDAPDomaindump
description: |
  Active Directory information dumper via LDAP, dumping AD users/computers/groups/policys/trusts.

command: |
  sudo ldapdomaindump ldap://192.168.122.41 -u "<domain\username>"
items:
  - Username
services:
  - LDAP
OS:
  - Linux
attack_types:
  - Enumeration
references:
  - https://github.com/dirkjanm/ldapdomaindump
---
