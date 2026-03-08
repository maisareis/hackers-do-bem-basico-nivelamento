# 🛠️ Comandos Úteis - Hackers do Bem (1ª Onda)

## 🐧 Linux

### Navegação e Arquivos
| Comando | Descrição |
|---------|-----------|
| `ls` | Lista arquivos e pastas |
| `ls -la` | Lista tudo, incluindo ocultos e permissões |
| `cd /caminho` | Muda de diretório |
| `cd ..` | Volta um nível |
| `pwd` | Mostra caminho atual |
| `mkdir nome` | Cria pasta |
| `rm nome` | Remove arquivo |
| `rm -rf pasta` | Remove pasta com tudo dentro (cuidado!) |
| `cp origem destino` | Copia arquivo |
| `cp -r origem destino` | Copia pasta |
| `mv origem destino` | Move ou renomeia |
| `cat arquivo` | Mostra conteúdo do arquivo |
| `nano arquivo` | Editor de texto simples |
| `touch arquivo` | Cria arquivo vazio |

### Permissões
| Comando | Descrição |
|---------|-----------|
| `chmod 755 arquivo` | Muda permissão (dono=rwx, grupo=r-x, outros=r-x) |
| `chmod u+x arquivo` | Adiciona execução para o dono |
| `chown usuario:grupo arquivo` | Muda dono e grupo |
| `chgrp grupo arquivo` | Muda apenas o grupo |

### Usuários
| Comando | Descrição |
|---------|-----------|
| `whoami` | Mostra usuário atual |
| `sudo comando` | Executa como root |
| `su -` | Vira root |
| `useradd -m nome` | Cria usuário com pasta home |
| `adduser nome` | Cria usuário (versão amigável) |
| `passwd nome` | Altera senha |
| `userdel nome` | Remove usuário |
| `groupadd nome` | Cria grupo |
| `usermod -aG grupo usuario` | Adiciona usuário a um grupo |

### Rede
| Comando | Descrição |
|---------|-----------|
| `ip a` | Mostra endereços IP |
| `ip r` | Mostra rota padrão |
| `ping 8.8.8.8` | Testa conectividade |
| `ss -tulpn` | Mostra portas abertas |
| `netstat -n` | Mostra conexões ativas |
| `curl site.com` | Faz requisição HTTP |
| `wget arquivo` | Baixa arquivo |
| `host nome.com` | Consulta DNS |
| `nslookup nome.com` | Consulta DNS |
| `dig nome.com` | Consulta DNS detalhada |

### Processos e Sistema
| Comando | Descrição |
|---------|-----------|
| `ps aux` | Lista processos |
| `top` | Monitora processos (ao vivo) |
| `htop` | Top melhorado |
| `kill PID` | Mata processo |
| `killall nome` | Mata por nome |
| `df -h` | Mostra espaço em disco |
| `du -sh pasta` | Mostra tamanho da pasta |
| `free -h` | Mostra memória RAM |
| `uname -a` | Info do sistema |
| `lsb_release -a` | Versão da distribuição |
| `systemctl status serviço` | Status do serviço |
| `systemctl start serviço` | Inicia serviço |
| `systemctl stop serviço` | Para serviço |
| `systemctl restart serviço` | Reinicia serviço |
| `journalctl -xe` | Logs do sistema |

### Pacotes (Debian/Ubuntu)
| Comando | Descrição |
|---------|-----------|
| `apt update` | Atualiza lista de pacotes |
| `apt upgrade` | Atualiza pacotes instalados |
| `apt install pacote` | Instala pacote |
| `apt remove pacote` | Remove pacote |
| `apt search termo` | Busca pacote |
| `dpkg -i arquivo.deb` | Instala .deb local |
| `snap install pacote` | Instala via snap |
| `flatpak install pacote` | Instala via flatpak |

### Pesquisa e Texto
| Comando | Descrição |
|---------|-----------|
| `grep "texto" arquivo` | Busca texto no arquivo |
| `grep -r "texto" pasta` | Busca recursivo |
| `\|` (pipe) | Conecta comandos (ex: `ls \| grep txt`) |
| `>` | Redireciona saída (sobrescreve) |
| `>>` | Redireciona saída (adiciona) |

---

# 🪟 Windows (CMD)

### Navegação e Arquivos
| Comando | Descrição |
|---------|-----------|
| `dir` | Lista arquivos e pastas |
| `cd \caminho` | Muda de diretório |
| `cd ..` | Volta um nível |
| `mkdir nome` | Cria pasta |
| `rmdir nome` | Remove pasta (vazia) |
| `rmdir /s /q nome` | Remove pasta com tudo |
| `del arquivo` | Remove arquivo |
| `copy origem destino` | Copia |
| `xcopy origem destino /e` | Copia pastas com subpastas |
| `move origem destino` | Move ou renomeia |
| `ren nome1 nome2` | Renomeia |
| `type arquivo` | Mostra conteúdo do arquivo |
| `notepad arquivo` | Abre no bloco de notas |

### Rede
| Comando | Descrição |
|---------|-----------|
| `ipconfig` | Mostra configurações IP |
| `ipconfig /all` | Mostra tudo (incluindo MAC) |
| `ping 8.8.8.8` | Testa conectividade |
| `tracert 8.8.8.8` | Mostra rota até o destino |
| `netstat -n` | Conexões ativas |
| `netstat -an` | Todas conexões e portas |
| `nslookup nome.com` | Consulta DNS |
| `arp -a` | Mostra tabela ARP |
| `route print` | Mostra tabela de roteamento |
| `telnet ip porta` | Testa conexão com porta |
| `ssh usuario@ip` | Conexão SSH (se tiver cliente) |

### Sistema
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
| `net user` | Lista usuários |
| `net user nome senha /add` | Cria usuário |
| `net localgroup` | Lista grupos |
| `net localgroup grupo nome /add` | Adiciona usuário ao grupo |

---

# 🌐 Redes (geral)

### Portas Comuns
| Porta | Protocolo | Serviço |
|------|-----------|---------|
| 20/21 | TCP | FTP |
| 22 | TCP | SSH |
| 23 | TCP | Telnet |
| 25 | TCP | SMTP |
| 53 | TCP/UDP | DNS |
| 67/68 | UDP | DHCP |
| 80 | TCP | HTTP |
| 110 | TCP | POP3 |
| 123 | UDP | NTP |
| 139 | TCP | NetBIOS |
| 143 | TCP | IMAP |
| 161 | UDP | SNMP |
| 389 | TCP | LDAP |
| 443 | TCP | HTTPS |
| 445 | TCP | SMB |
| 3389 | TCP | RDP |

### Conceitos
- **/24** = 255.255.255.0 (256 IPs, 254 válidos)
- **/16** = 255.255.0.0 (65.536 IPs)
- **/8** = 255.0.0.0 (16.777.216 IPs)
- **IP Privados RFC1918**: 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16
- **Loopback**: 127.0.0.1
- **Broadcast**: último IP da rede

---

# 🔧 Ferramentas

### Scan e Exploração
| Ferramenta | Uso básico |
|------------|------------|
| **nmap** | `nmap -sV 192.168.1.1` |
| **nmap** | `nmap -p- 192.168.1.1` |
| **nmap** | `nmap -A 192.168.1.1` |
| **netcat** | `nc -zv ip porta` |
| **netcat** | `nc -lvnp 443` |
| **wireshark** | Análise de pacotes (GUI) |
| **tcpdump** | `tcpdump -i eth0` |

### HTTP
| Ferramenta | Uso básico |
|------------|------------|
| **curl** | `curl http://site.com` |
| **curl** | `curl -X POST -d "dado" http://site.com` |
| **wget** | `wget http://site.com/arquivo` |
| **whatweb** | `whatweb site.com` |

### Senhas e Hashes
| Ferramenta | Uso básico |
|------------|------------|
| **hashcat** | `hashcat -m 0 hash.txt wordlist.txt` |
| **john** | `john --wordlist=wordlist.txt hash.txt` |
| **hydra** | `hydra -l user -P wordlist.txt ssh://ip` |

---

# 📝 Scripts Rápidos

## Bash - Verificar portas abertas
```bash
#!/bin/bash
host="127.0.0.1"

for porta in 22 80 443 3389
do
  nc -zv "$host" "$porta" 2>/dev/null && echo "Porta $porta aberta" || echo "Porta $porta fechada"
done
```

## Bash - Monitorar log de autenticação
```bash
#!/bin/bash
tail -f /var/log/auth.log | grep "Failed password"
```

## PowerShell - Verificar conexões ativas
```powershell
Get-NetTCPConnection | Where-Object {$_.State -eq "Established"}
```

## PowerShell - Listar processos suspeitos
```powershell
Get-Process | Where-Object { $_.CPU -gt 50 } | Format-Table Name, CPU, ID
```

## Bash - Backup simples
```bash
#!/bin/bash
DATA=$(date +%Y%m%d)

tar -czf backup_$DATA.tar.gz /home/usuario/documentos

echo "Backup concluído: backup_$DATA.tar.gz"
```

## Bash - Verificar espaço em disco
```bash
#!/bin/bash
df -h | grep -E '^/dev/' | while read linha
do
  echo "Espaço em disco: $linha"
done
```
