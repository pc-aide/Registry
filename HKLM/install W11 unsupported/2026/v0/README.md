# install W11 unsupported 

## steps
1. ctrl + shift + F10 - cmd 
2. hklm\system\setup\<NewKey>
3.   name : LabConfig
<img src="https://i.imgur.com/jAFG5mu.png">

4. newDWORD 32 bit :
    * **Name** : BypassTPMCheck & value = 1
    * **Name** : BypassSecureBootCheck & value = 1
<img src="https://i.imgur.com/VVxKGt5.png">

<img src="https://i.imgur.com/lC8Acxu.png">

<img src="https://i.imgur.com/Qwtk8Dy.png">
