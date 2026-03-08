# Aula 6 – Transferência de Arquivos

## 📌 Servidores
- Computadores com alto poder de processamento e armazenamento
- Escaláveis
- Atuam em LAN ou WAN
- Arquitetura cliente/servidor

## 📌 NAS (Network Attached Storage)
- Exclusivo para armazenamento e compartilhamento
- Backup de dados
- Pode suportar milhares de computadores
- Sistema operacional embarcado
- Replicação de dados (segurança)

## 📌 Protocolos

### SMB/CIFS (Server Message Block)
- Compartilhamento de arquivos em rede
- Porta 445 (Windows 2000+)
- Porta 139 (versões antigas)
- Usa TCP/IP
- Requer autenticação

### FTP (File Transfer Protocol)
- Porta 21 (controle), 20 (dados)
- Dois canais: comando e dados
- Modos ativo e passivo
- Pode ser anônimo ou autenticado

### TFTP (Trivial FTP)
- Porta 69
- UDP (não confiável)
- Simples, sem autenticação
- Usado para boot de rede, backup de switches

### Torrent / P2P
- Modelo descentralizado
- **Seed:** quem compartilha
- **Peer:** quem baixa
- BitTorrent é o protocolo mais comum