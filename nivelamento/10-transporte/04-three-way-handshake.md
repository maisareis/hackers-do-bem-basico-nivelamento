# Aula 4 – Three-way Handshake

## 📌 O que é
- Processo de estabelecimento de conexão TCP
- 3 passos antes de enviar dados

## 📌 Passo a passo

**1. Cliente → Servidor: SYN**
- Cliente envia segmento com flag SYN ativa
- Número de sequência inicial (ex: 1000)
- "Vamos nos conectar?"

**2. Servidor → Cliente: SYN-ACK**
- Servidor responde com SYN e ACK
- Número de sequência do servidor (ex: 2000)
- Confirma número do cliente (ACK = 1001)
- "Ok, estou pronto. Confirme."

**3. Cliente → Servidor: ACK**
- Cliente envia ACK confirmando
- ACK = 2001
- Conexão estabelecida

## 📌 Resultado
- Conexão bidirecional estabelecida
- Dados podem ser enviados
- Ambos sabem que o outro está pronto

## 📌 Visualização

Cliente                 Servidor
   |---- SYN (seq=1000) ---->|
   |<--- SYN-ACK (seq=2000, ack=1001) ----|
   |---- ACK (ack=2001) ---->|
   |                          |
   |======== dados =========>|

## 📌 Flags TCP
- **SYN** (Synchronize) → iniciar conexão
- **ACK** (Acknowledgment) → confirmar recebimento
- **FIN** (Finish) → finalizar conexão
- **RST** (Reset) → resetar conexão
- **PSH** (Push) → enviar dados imediatamente
- **URG** (Urgent) → dados urgentes

## 📌 Números de sequência
- Iniciais aleatórios (ISN - Initial Sequence Number)
- Incrementam a cada byte enviado
- Permite controle de ordem e confirmação