# Aula 6 – Protocolo UDP

## 📌 Características
- **Não orientado à conexão** → envia direto
- **Não confiável** → sem confirmação (ACK)
- **Não reenvia dados perdidos**
- **Não reorganiza datagramas**
- **Leve e rápido**

## 📌 Analogia
- TCP = carta registrada (confirmação, rastreio)
- UDP = panfleto jogado na multidão (sem garantia)

## 📌 Cabeçalho UDP
- Apenas 8 bytes
- 4 campos:
  - Porta origem (16 bits)
  - Porta destino (16 bits)
  - Tamanho (16 bits)
  - Checksum (16 bits)

## 📌 Quando usar UDP
- Streaming de vídeo/áudio (perda pequena não importa)
- VoIP (telefonia IP)
- Jogos online (velocidade > confiabilidade)
- DNS (consultas rápidas)
- DHCP
- SNMP
- TFTP (Trivial FTP)

## 📌 Exemplos
- Assistir vídeo ao vivo
- Jogar online
- Ligação por WhatsApp/Teams