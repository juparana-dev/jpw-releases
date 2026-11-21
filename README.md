# JupWatcher - releases

Somente artefatos instaláveis aprovados, sem credenciais. O token do CGE é pedido na instalação, com entrada oculta.

## Versão atual: JPW22.1 `0.1.0-homologation.22.1`

PowerShell (Windows PowerShell 5.1), sem alterar a política de execução:

```powershell
$f="$env:TEMP\jpw-install.cmd"; curl.exe -fsSLo $f https://github.com/juparana-dev/jpw-releases/releases/download/jpw22-v0.1.0-homologation.22.1/jpw-install.cmd; if((Get-FileHash $f).Hash -eq '7b1fe41306008c9ef3de27e9bc1e5c6147fd811af6d78174a807429f7e7d281d'){& $f}else{'JPW_BOOTSTRAP=HASH_MISMATCH'}
```

Hashes e notas: https://github.com/juparana-dev/jpw-releases/releases/tag/jpw22-v0.1.0-homologation.22.1

Sem download: coloque `JupWatcher-JPW22.zip` ao lado de `jpw-install.cmd` e execute o `.cmd`. Depois: `jpw status`, `jpw setup`, `jpw check`.

Versões anteriores permanecem publicadas (pré-lançamento `jpw22-v0.1.0-homologation.22`).
