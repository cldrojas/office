# How to install office correctly

![cldrojas_logo](https://github.com/cldrojas/portfolio/blob/master/public/img/Daniel%20Rojas%20Brand.png)

## Uninstall Office previous installations

To install office correctly, first you need to uninstall previous versions of windows and license keys asociated to that software

Support and Recovery Asistant is the better tool for accomplish that task. Created by Microsoft

### Installing SaRA

Execute SaRA.exe, then click on install. Agree terms, select your office previous installation and click _uninstall_

Restart your computer

### Download links

- https://www.microsoft.com/en-us/download/confirmation.aspx?id=100607
- https://support.microsoft.com/es-es/office/desinstalar-office-de-un-equipo-pc-9dd49b83-264a-477a-8fcc-2fdf5dbf61d8

## Install Office 2021

Download and unzip Microsoft Office 2021, then execute setup.exe file depending on your system architecture

- https://drive.google.com/file/d/1zGBx3lodXCjDOEc9TeRIPqbcE_Ob3v9N/view

Close your app and go to office installation folder within a terminal

```
cd /d %ProgramFiles%\Microsoft Office\Office16
```

Install offline license

```
for /f %x in ('dir /b ..\root\Licenses16\ProPlus2021VL_KMS*.xrm-ms') do cscript ospp.vbs /inslic:"..\root\Licenses16\%x"
```

Install generated product keys set

```
cscript ospp.vbs /setprt:1688
cscript ospp.vbs /unpkey:6F7TH >nul
cscript ospp.vbs /inpkey:FXYTK-NJJ8C-GB6DW-3DYQT-6F7TH
cscript ospp.vbs /sethst:kms.srv.crsoo.com
cscript ospp.vbs /act
```

Close your terminal and you are ready to go. Congrats, office 2021 installed successfuly!
