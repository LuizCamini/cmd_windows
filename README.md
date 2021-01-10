# cmd_windows

#### Abrir o CMD
```shell
tecla windows + R e digite CMD
```

#### Listar Todos os Programas Windows
```shell
wmic /output:c:\InstalledSoftwareList.txt product get name, version
```

### Melhorar Desempenho do Windows

#### Verificar erros no Disco (Requer CMD ou POWERSHELL em modo Admin):
```shell
CHKDSK /R
```

#### Repara arquivos protegidos do windows (Requer CMD ou POWERSHELL em modo Admin):
```shell
sfc /scannow
```

#### Repara arquivos corrompidos ou ausentes do S.O(Requer CMD ou POWERSHELL em modo Admin, valido para versoes acima do windows 8):
```shell
DISM /Online /Cleanup-image /Restorehealth

```

