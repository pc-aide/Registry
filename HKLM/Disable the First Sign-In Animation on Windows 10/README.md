Windows Registry Editor Version 5.00
 
; created by Brady Gavin
; for How-To Geek
; article: https://www.howtogeek.com/492003/how-to-disable-the-first-sign-in-animation-on-windows-10/ 
; https://i.imgur.com/CEjvCyd.png
 
[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon]
"EnableFirstLogonAnimation"=dword:00000000
