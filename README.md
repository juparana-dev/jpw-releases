# JupWatcher — releases

Somente artefatos instaláveis aprovados, sem credenciais. O token do CGE é pedido na instalação, com entrada oculta.

## JPW22 `0.1.0-homologation.22` (candidata à homologação)

PowerShell, sem alterar a política de execução:

```powershell
$f="$env:TEMP\jpw-install.cmd"; curl.exe -fsSLo $f https://github.com/juparana-dev/jpw-releases/releases/download/jpw22-v0.1.0-homologation.22/jpw-install.cmd; if((Get-FileHash $f).Hash -eq '741e24c32ae226319b3496dba5adb2f1de2fed5675c3cf6bd0e6e01cb16902ba'){& $f}else{'JPW_BOOTSTRAP=HASH_MISMATCH'}
```

| Arquivo | SHA-256 |
| --- | --- |
| `JupWatcher-JPW22.zip` | `786810fde6e91a6a932983d10523a92ce8df0739fa34da6ccb79185aaac3c1ec` |
| `jpw-install.cmd` | `741e24c32ae226319b3496dba5adb2f1de2fed5675c3cf6bd0e6e01cb16902ba` |

Sem acesso de download: coloque `JupWatcher-JPW22.zip` ao lado de `jpw-install.cmd` e execute o `.cmd`.
Depois de instalado: `jpw status`, `jpw setup`, `jpw check`.