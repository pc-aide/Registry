# Adobe-AcrobatReaderDC22.001.20169_x32

---

## disable the prompt "Make Adobe Acrobat my default PDF application
````ps1
# SRC : https://helpx.adobe.com/ca/acrobat/kb/disable-prompt-to-make-acrobat-my-default.html
Get-Item 'HKCU:\Software\Adobe\Acrobat Reader\DC\AVAlert\cCheckbox\' |
fl Property,valueCount

Property   : {iAppDoNotTakePDFOwnershipAtLaunch}
ValueCount : 1
````
