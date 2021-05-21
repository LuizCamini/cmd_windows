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
#### Listar pastas de unidade, ordenado e gerar arquivo com a listagem:

```shell
dir /s /b /OG /AD lista.txt
```
#### Listar pastas e subpastas de unidade, ordenado e gerar arquivo com a listagem:
```shell
dir /s /b /o:g /ad /on > lista2.txt
```

#### Acesso aos serviços do Windows
```shell
services.msc
```

#### Acesso ao Gerenciador de tarefas
```shell
taskmgr
```

#### Acesso ao Painel de Control
```shell
control panel
```

#### Acesso ao controle de impressoras
```shell
control printers
```

#### Acesso ao controle de Pastas
```shell
control folders
```


#### Abre a janela para adicionar ou remover programas
```shell
appwiz.cpl
```

#### Abre a janela de informações do sistema, onde é possível obter um resumo dos componentes do PC, bem como obter detalhes sobre conflitos
```shell
msinfo32
```

#### Habilitar Arquivos com mesmo nome na mesma Pasta (Sensitive Case para arquivos)
```shell
fsutil.exe file setCaseSensitiveInfo c:\users\nome.usuario\Documents\teste enable
```

##Comandos PowerShell  
```shell

```
#### LISTAR PROCESSOS  
```shell
get-process sqlserver*
```


#### VARIAVEL USAR $  
```shell
$VARIAVEL
```
#### exemplo acessando o primeiro item da lista  
```shell
$VARIAVEL[0]
```

#### LISTAR ESPAÇO EM DISCO  
```shell
get-WmiObject Win32_Volume
get-WmiObject Win32_Volume | select Name, capacity, freespace
```


- wiaacmgr:    			Abre o assistente de câmera ou scanner
- migwiz:      			Abre o assistente de transferência de definições e arquivos
- fsquirt:     			Abre o assistente de transferência de arquivo Bluetooth
- hdwwiz.cpl:  			Abre o gerenciador de dispositivos do Windows
- calc: 		 		Abre Calculadora
- wscui.cpl:   			Abre a central de segurança e manutenção do Windows, onde é possível ver se está tudo bem com o Firewall, software antivírus e mais
- certmgr.msc: 			Abre a central de visualização e gerenciamento de certificados
- telnet: 	 			Se instalado, abre o cliente Telnet do Windows
- ipconfig /flushdns: 	Apaga informações de DNS do protocolo IP
- ipconfig /release: 	"Libera" o endereço IP atribuído por DHCP de uma determinada interface
- ipconfig /displaydns: Ver DNS
- ipconfig /all: 		Visualizar todas as informações de rede
- ipconfig /setclassid: Modifica o Class ID do DHCP
- ipconfig: 			Ver informações do protocolo IP
- rsop.msc: 			Abre console de gerenciamento do conjunto de políticas resultantes
- joy.cpl: 				Abre painel de controladores de jogo
- secpol.msc: 			Abre gerenciador de políticas de segurança local
- logoff: 				Efetua logoff da conta autenticada no momento no Windows
- eudcedit: 			Inicia o editor de caracteres privados
- regedit: 				Abre o editor de registro do Windows


- shutdown: 			Desliga o sistema e o computador
- dir: 					Exibe uma lista de arquivos e subpastas de uma pasta específica
- explorer: 			Abre o explorador de arquivos
- dxdiag: 				Ferramenta de diagnóstico do DirectX
- wabmig: 				Ferramenta de importação de livro de endereços
- mrt: 					Abre a ferramenta de remoção de software mal-intencionado do Windows
- control admintools: 	Acessa as ferramentas administrativas do Windows
- firewall.cpl: 		Abre o painel de firewall do Windows, onde é possível checar as configurações atuais da proteção, bem como definir suas políticas de bloqueio
- fonts: 				Fontes
- compmgmt.msc: 		Abre o painel de gerenciamento do computador, onde é possível agendar tarefas, definir pasta compartilhadas, entre outras coisas
- diskmgmt.msc: 		Abre o gerenciamento de discos do Windows. Aqui é possível particionar os discos rígidos, redimensioná-los etc


- devmgmt.msc: 			  Também acessa o gerenciador de dispositivos do sistema
- diskpart: 			  Acessa o gerenciador de partições do disco rígido
- taskmgr: 				  Abre o gerenciador de tarefas, aquele mesmo que você costuma abrir pressionando CTRL + SHIFT + ESC no teclado
- utilman: 				  Abre a central de facilidade de acesso do Windows, onde é possível determinar como o sistema se apresentará a pessoas com dificuldades motoras, visuais e/ou auditivas
- verifier: 			  Gerenciador de verificação de drivers
- iexpress: 			  Abre o wizard para criação de arquivos executáveis (.exe)
- control printers: 	  Abre o gerenciador de dispositivos e impressoras, onde é possível adicionar dispositivos USB, Bluetooth e impressoras
- wmimgmt.msc: 			  Gerenciador de infraestrutura do Windows
- mobsync: 				  Abre a central de sincronização do sistema
- mstsc: 				  Abre o console de conexão de área de trabalho remota
- ncpa.cpl: 			  Abre o gerenciador de conexões de rede
- control netconnections: Abre o gerenciador de conexões de rede
- cleanmgr: 			  Executa limpeza de disco
- cmd: 					  Prompt de comando
- rasphone: 			  Para os que ainda usam, abre a lista telefônica
- wab: 					  Também algo antiquado, um livro de endereços
- charmap: 				  Abre o mapa de caracteres
- dialer: 				  Acessa o discador telefônico
- access.cpl: 			  Microsoft Access, se estiver instalado
- excel: 				  Microsof Excel, se estiver instalado
- frontpg: 				  Microsoft Frontpage, se estiver instalado
- mspaint: 				  Microsoft Paint, para a garotada

- powerpnt: 			Microsoft Powerpoint, se estiver instalado
- winword: 				Microsoft Word, se estiver instalado
- notepad: 				Bloco de notas
- control folders: 		Abre as opções do explorador de arquivos, onde você pode definir se quer exibir pastas e arquivos ocultos, etc.
- intl.cpl: 			Abre as configurações de região e idioma do Windows
- control: 				Painel de controle
- pbrush: 				Alternativa para abrir o Microsoft Paint (antes também conhecido como Paint Brush)
- fsmgmt.msc: 			Lista as pastas compartilhadas
- perfmon: 				Abre o monitor de desempenho do sistema
- perfmon.msc: 			Abre o monitor de desempenho do sistema
- telephon.cpl: 		Opções de modem e telefone
- gpedit.msc: 			Editor de políticas de grupo local
- powercfg.cpl: 		Inicia as opções de energia, onde é possível definir o perfil de consumo energético do computador
- control color: 		Abre menu de definição de aparência e cores do Windows
- inetcpl.cpl: 			Abre as configurações de internet do sistema
- timedate.cpl: 		Propriedades de data e hora
- mmsys.cpl: 			Configurações de som do Windows
- control desktop: 		Ajustes de resolução de tela/monitor
- desk.cpl:				Ajustes de resolução de tela/monitor
- main.cpl:				Acessa as propriedades e definições do mouse
- control mouse:		Acessa as propriedades e definições do mouse
- sysdm.cpl: 			Abre as propriedades do sistema
- control keyboard: 	Propriedades e configurações do teclado
- syskey: 				Painel de proteção da base de dados dos usuários Windows
- sfc /scanboot: 		Analisa a inicialização do sistema
- sfc /scanonce: 		Analisa a próxima inicialização do sistema
- sfc /scannow: 		Analisa a inicialização imediatamente
- sfc /revert: 			Restabelece as configurações de inicialização de fábrica
- QuickTime.cpl: 		Abre as configurações do QuickTime, se ele estiver instalado
- realplay: 			Abre as configurações do Real Player, se ele estiver instalado
- services.msc: 		Abre o gerenciador de serviços do Windows


- dcomcnfg: 			Serviços de componente
- control schedtasks: 	Gerenciador de tarefas agendadas do sistema
- osk: 					Abre o teclado virtual do Windows
- control fonts: 		Fontes
- tweakui: 				Abre o Tweak UI, se estiver instalado
- msconfig: 			Utilitário de configuração do sistema, onde é possível definir quais programas e serviços são inicializados com o Windows e mais
- cliconfg: 			Utilitário de rede para clientes SQL Server
- sfc: 					Utilitário de verificação de integridade dos arquivos do sistema
- chkdsk: 				Utilitrário de verificação de integridade do disco rígido
- lusrmgr.msc: 			Gerenciador de usuários e grupos locais do sistema
- sigverif: 			Verificador de assinaturas de arquivos
- javaws: 				Visualizador de aplicações Java, se estiver instalado
- eventvwr.msc: 		Visualizador de eventos do Windows, uma espécie de log do sistema
- magnify: 				Lupa
- wmplayer: 			Windows Media Player
- write: 				Wordpad