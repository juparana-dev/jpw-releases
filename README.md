# JupWatcher - releases

Somente artefatos instaláveis aprovados, sem credenciais. O token do CGE é pedido na instalação, com entrada oculta.

## Versão atual: JPW22.2 `0.1.0-homologation.22.2`

PowerShell (Windows PowerShell 5.1), sem alterar a política de execução:

```powershell
$f="$env:TEMP\jpw-install.cmd"; curl.exe -fsSLo $f https://github.com/juparana-dev/jpw-releases/releases/download/jpw22-v0.1.0-homologation.22.2/jpw-install.cmd; if((Get-FileHash $f).Hash -eq '468ba1d52b840d47b043b3cb3a64a67403169112ef7d8a263c7ed70009f817bd'){& $f}else{'JPW_BOOTSTRAP=HASH_MISMATCH'}
```

Hashes e notas: https://github.com/juparana-dev/jpw-releases/releases/tag/jpw22-v0.1.0-homologation.22.2

Depois: `jpw status`, `jpw setup`, `jpw check`. Versões anteriores permanecem publicadas.
