# Aula 2 – Portas

## 📌 O que são portas
- Identificadores de serviços na camada de transporte
- Permitem múltiplas conexões simultâneas
- Números de 0 a 65535

## 📌 Analogia
- Endereço IP = rua/CEP
- Porta = número do apartamento

## 📌 Faixas de portas
- **0 a 1023:** portas bem conhecidas (well-known)
  - Ex: 80 (HTTP), 443 (HTTPS), 22 (SSH)
- **1024 a 49151:** portas registradas
- **49152 a 65535:** portas dinâmicas/efêmeras

## 📌 Portas comuns

| Porta | Protocolo | Serviço |
|-------|-----------|---------|
| 20/21 | TCP | FTP |
| 22 | TCP | SSH |
| 23 | TCP | Telnet |
| 25 | TCP | SMTP |
| 53 | TCP/UDP | DNS |
| 67/68 | UDP | DHCP |
| 80 | TCP | HTTP |
| 110 | TCP | POP3 |
| 123 | UDP | NTP |
| 143 | TCP | IMAP |
| 161 | UDP | SNMP |
| 389 | TCP | LDAP |
| 443 | TCP | HTTPS |
| 445 | TCP | SMB |
| 3389 | TCP | RDP |

## 📌 Arquivo de serviços
- **Windows:** C:\Windows\System32\drivers\etc\services
- **Linux:** /etc/services