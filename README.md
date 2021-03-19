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

#### Reparar arquivos corrompidos ou ausentes do S.O(Requer CMD ou POWERSHELL em modo Admin, comando valido apenas para versoes acima do windows 8):
```shell
DISM /Online /Cleanup-image /Restorehealth
```
#### Listar pastas de unidade ordenando e gera arquivo com a listagem:

```shell
dir /s /b /OG /AD lista.txt
```
#### Listar pastas e subpastas de unidade ordenando e gera arquivo com a listagem:
```shell
dir /s /b /o:g /ad /on > lista2.txt
```

