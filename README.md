# JPW22.5

Terminal

```powershell
$f="$env:TEMP\jpw-install.cmd"; curl.exe -fsSLo $f https://github.com/juparana-dev/jpw-releases/releases/download/jpw22-v0.1.0-homologation.22.5/jpw-install.cmd; if((Get-FileHash $f).Hash -eq 'e40941525c21fff87cb4b3020e5d6dcdb09c31d1501927d2259ff0aafee49020'){& $f}else{'JPW_BOOTSTRAP=HASH_MISMATCH'}
```
