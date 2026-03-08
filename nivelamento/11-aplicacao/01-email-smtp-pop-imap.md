# Aula 1 – E-mail: SMTP, POP3 e IMAP

## 📌 História
- Primeiro e-mail: 1971 (Ray Tomlinson, ARPANET)
- Primeiro spam: 1978 (Gary Thuerk)
- Hotmail: 1996 (primeiro webmail gratuito)
- 4,3 bilhões de contas (2022)

## 📌 Protocolos de e-mail

### SMTP (Simple Mail Transfer Protocol)
- Envio de mensagens
- Porta 25 (sem criptografia)
- Porta 587 (com criptografia - TLS)
- Cabeçalho + corpo da mensagem
- Servidor armazena e encaminha

### POP3 (Post Office Protocol)
- Download de mensagens
- Baixa e apaga do servidor (padrão)
- Porta 110 (sem criptografia)
- Porta 995 (com criptografia)

### IMAP (Internet Message Access Protocol)
- Sincronização de mensagens
- Mantém no servidor
- Acesso de múltiplos dispositivos
- Porta 143 (sem criptografia)
- Porta 993 (com criptografia)

## 📌 Comparação POP3 x IMAP
- **POP3:** mensagens baixadas, offline, dispositivo único
- **IMAP:** mensagens no servidor, online, múltiplos dispositivos