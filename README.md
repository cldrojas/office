# How to install Office

![cldrojas_logo](https://user-images.githubusercontent.com/16184660/180892336-66348c9f-0ee5-4397-bd56-67d4123494c2.png)

## Uninstall Office previous installations

To install office correctly, first you need to uninstall previous versions and license keys asociated to that software  
Support and Recovery Asistant is the best tool for accomplish that. Created by Microsoft

### Installing SaRA

Execute SaRA.exe, then click on install. Agree terms, select your office previous installation and click _uninstall_

Restart your computer

### Download links

- [descarga](https://www.microsoft.com/en-us/download/confirmation.aspx?id=100607)
- [Guia](https://support.microsoft.com/es-es/office/desinstalar-office-de-un-equipo-pc-9dd49b83-264a-477a-8fcc-2fdf5dbf61d8)

## Install Office 2021

Download and unzip Microsoft Office 2021, then execute setup.exe file depending on your system architecture

- [descarga office](https://drive.google.com/file/d/1zGBx3lodXCjDOEc9TeRIPqbcE_Ob3v9N/view)

Close your app and go to office installation folder within a terminal

`Cierra la aplicación y abre powershell como administrador, ahí pega la siguiente linea`

```
cd /d %ProgramFiles%\Microsoft Office\Office16
```

Install offline license
 `pega las siguientes lineas en orden`
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
`hasta aqui ya deberías tener office instalado y activado, cierra powershell`
Close your terminal and you're ready to go. Congrats, office 2021 was installed successfuly!


# Free antivirus Avast
## Download and install

- https://www.avast.com/es-us/free-antivirus-download#pc

   Uncheck install avast Secure browser  
   Go to personalize and check all options on left column and last option on the right side  
   Click continue to finalize configuring avast free  
   Select free option and that's it
