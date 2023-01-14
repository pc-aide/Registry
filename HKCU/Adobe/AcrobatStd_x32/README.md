# Adobe-AcrobatStd__x32

---

## disable the prompt "Make Adobe Acrobat my default PDF application
````ps1
# SRC : https://helpx.adobe.com/ca/acrobat/kb/disable-prompt-to-make-acrobat-my-default.html
# Test :
# New key
New-item "HKLM:\SOFTWARE\Adobe\Adobe Acrobat\DC\AVAlert" -Name cCheckbox -Force

# New value
# Syntax : \Adobe\<ProductName>\<version>\AVAlert\cCheckbox
New-ItemProperty "HKLM:\SOFTWARE\Adobe\Adobe Acrobat\DC\AVAlert\cCheckbox\" -Name iAlwaysEnablePDFMAddin -Value 1 -Type dword -Force
````
