# Quakbot
Ricevuta in data 15/03/2022, analisi preliminare


### Path
Phishing > .zip > .xls > dump to .dll > regsvr32 

### Files and hashes
```
limtapilaios.zip       fc8f57a368f620b74ea1ecababadf9b5
limtapilaios.xls
rvr1.dll               83e7efb88a396798e7c7bb088ed5e1be
```

### Process tree
```
C:\Windows\System32\rundll32.exe C:\Users\USER\AppData\Local\Temp\rvr1.dll,#1
    C:\Windows\SysWOW64\explorer.exe
        C:\Windows\system32\schtasks.exe /Create /RU "NT AUTHORITY\SYSTEM" /tn mnjgxjno /tr "regsvr32.exe -s C:\Users\USER\AppData\Local\Temp\rvr1.dll" /SC ONCE /Z /ST 16:42 /ET 16:54
```

#### Links
https://tria.ge/220315-lnf6jahgc7/behavioral2
