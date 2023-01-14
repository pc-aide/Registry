# Adobe-AcrobatStd__x32

---

## disable the prompt "Make Adobe Acrobat my default PDF application
````ps1
# SRC : https://helpx.adobe.com/ca/acrobat/kb/disable-prompt-to-make-acrobat-my-default.html
# Practique\AdobeAcrobatReaderDC-22.001.20169_x32 :
Get-Item 'HKCU:\Software\Adobe\Acrobat Reader\DC\AVAlert\cCheckbox\' |
fl Property,valueCount

Property   : {iAppDoNotTakePDFOwnershipAtLaunch}
ValueCount : 1

# Test10 :
# New key
New-item "HKLM:\SOFTWARE\Adobe\Acrobat Reader\DC\AVAlert\" -Name cCheckbox -Force

# New value
# Syntax : \Adobe\<ProductName>\<version>\AVAlert\cCheckbox
New-ItemProperty "HKLM:\Software\Adobe\Acrobat Reader\DC\AVAlert\cCheckbox\" `
  -Name iAlwaysEnablePDFMAddin -Value 1 -Type dword -Force  
  
# result after test: fail
````
