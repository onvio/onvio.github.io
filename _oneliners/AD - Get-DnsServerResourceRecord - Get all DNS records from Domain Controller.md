---
title: |
  Get all DNS records from Domain Controller with Domain Admin
description: |
  The Get-DnsServerResourceRecord cmdlet gets the following information for a specified resource record from a Domain Name System (DNS) zone:

  	HostName

  	RecordType

  	RecordClass

  	TimeToLive

  	Timestamp

  	RecordData

command: |
  Get-DnsServerResourceRecord -ZoneName <AD>
items:
  - Password
  - Username
  - Shell
OS:
  - Windows
attack_types:
  - Enumeration
references:
  - https://github.com/MicrosoftDocs/windows-powershell-docs/blob/main/docset/winserver2012-ps/dnsserver/Get-DnsServerResourceRecord.md
---
