# Aula 7 – Comparativo TCP x UDP

## 📌 Tabela comparativa

| Característica | TCP | UDP |
|----------------|-----|-----|
| Conexão | Orientado | Não orientado |
| Confiabilidade | Sim (ACK) | Não |
| Reenvio | Sim | Não |
| Ordenação | Sim | Não |
| Controle de fluxo | Sim | Não |
| Cabeçalho | 20-60 bytes | 8 bytes |
| Velocidade | Mais lento | Mais rápido |
| Uso | Dados importantes | Tempo real |

## 📌 Aplicações típicas

### TCP
- HTTP/HTTPS (navegação)
- SMTP/POP/IMAP (e-mail)
- FTP (transferência de arquivos)
- SSH (acesso remoto seguro)
- Banco de dados

### UDP
- DNS (consultas)
- DHCP (atribuição de IP)
- VoIP (telefonia)
- Streaming de vídeo
- Jogos online
- SNMP (monitoramento)
- TFTP (transferência simples)

## 📌 Algumas aplicações usam ambos
- Discord: 
  - TCP 443 → chat de texto
  - UDP 45000-60000 → chat de voz

## 📌 Escolha
- **TCP:** quando não pode perder dados
- **UDP:** quando velocidade é mais importante que confiabilidade