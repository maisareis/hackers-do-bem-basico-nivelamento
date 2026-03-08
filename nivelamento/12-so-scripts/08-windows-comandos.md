# Aula 8 – Windows: Comandos

## 📌 Navegação e arquivos

| Comando | Descrição |
|---------|-----------|
| `dir` | Lista arquivos e pastas |
| `cd \caminho` | Muda de diretório |
| `cd ..` | Volta um nível |
| `mkdir nome` | Cria pasta |
| `rmdir nome` | Remove pasta (vazia) |
| `rmdir /s /q nome` | Remove pasta com tudo |
| `del arquivo` | Remove arquivo |
| `copy origem destino` | Copia arquivo |
| `xcopy origem destino /e` | Copia pastas com subpastas |
| `move origem destino` | Move ou renomeia |
| `ren nome1 nome2` | Renomeia |
| `type arquivo` | Mostra conteúdo |
| `type con > arquivo` | Cria arquivo com teclado (Ctrl+Z) |

## 📌 Rede

| Comando | Descrição |
|---------|-----------|
| `ipconfig` | Configurações IP |
| `ipconfig /all` | Mostra tudo (incluindo MAC) |
| `ping 8.8.8.8` | Testa conectividade |
| `tracert 8.8.8.8` | Mostra rota |
| `netstat -n` | Conexões ativas |
| `netstat -an` | Todas conexões e portas |
| `nslookup nome.com` | Consulta DNS |
| `arp -a` | Tabela ARP |
| `route print` | Tabela de roteamento |

## 📌 Sistema

| Comando | Descrição |
|---------|-----------|
| `systeminfo` | Informações do sistema |
| `tasklist` | Lista processos |
| `taskkill /PID 1234` | Mata processo por PID |
| `taskkill /IM nome.exe /F` | Mata processo por nome |
| `chkdsk` | Verifica disco |
| `sfc /scannow` | Verifica arquivos do sistema |
| `shutdown /r` | Reinicia |
| `shutdown /s` | Desliga |
| `whoami` | Usuário atual |

## 📌 Usuários

| Comando | Descrição |
|---------|-----------|
| `net user` | Lista usuários |
| `net user nome senha /add` | Cria usuário |
| `net user nome /del` | Remove usuário |
| `net localgroup` | Lista grupos |
| `net localgroup grupo nome /add` | Adiciona ao grupo |