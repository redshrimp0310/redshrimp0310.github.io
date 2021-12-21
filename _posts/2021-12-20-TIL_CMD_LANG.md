---
title:  "Change Language of Command Prompt in Windows"
excerpt: "Wanted to change English Command Line interface to Korean due to the unreadable characters"

categories:
  - CMD
tags:
  - [TIL, CMD, Language]

toc: true
toc_sticky: true
 
date: 2021-12-20
last_modified_at: 2021-12-20
---

## DESCRIPTION
Wanted to change English Command Line interface to Korean due to the unreadable characters as below.

![cmd1korean](/img/cmd/cmd1.jpg)

## RESOLUTION
* Checked the current active code first using 'CHCP' command which is used to supplement the the international keyboard & character set information.

![cmd1korean](/img/cmd/cmd2.jpg)

* Changed to Active code page 949(Korean). However, this is a temporary solution. It goes back to the default active code setting once CMD has been closed.

![cmd1korean](/img/cmd/cmd3.jpg)

* In order for the change to be made permanently, Go to [HKEY_LOCAL_MACHINE\Software\Microsoft\Command Processor] in regedit and add new String Value named 'Autorun' with 'chcp 949 value'.

![cmd1korean](/img/cmd/cmd4.jpg)

![cmd1korean](/img/cmd/cmd5.jpg)

## REFERENCE
* https://m-falcon.tistory.com/363
* https://rachel921.tistory.com/17
* https://stackoverflow.com/questions/57131654/using-utf-8-encoding-chcp-65001-in-command-prompt-windows-powershell-window
* https://stackoverflow.com/questions/7432545/change-codepage-in-cmd-permanently