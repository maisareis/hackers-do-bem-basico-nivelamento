# Aula 5 – Janelamento (Controle de Fluxo)

## 📌 O que é
- Controle de quantos segmentos podem ser enviados sem confirmação
- Evita sobrecarregar o receptor
- Receptor informa o tamanho da janela

## 📌 Funcionamento
1. Emissor envia janela de segmentos
2. Receptor confirma recebimento (ACK)
3. Receptor informa próximo número esperado
4. Emissor pode enviar mais

## 📌 Exemplo
- Janela = 3 segmentos
- Envia 1, 2, 3
- Receptor confirma 1, 2, 3
- Envia 4, 5, 6...

## 📌 Se perder um segmento
- Receptor não confirma o perdido
- Emissor reenvia a janela toda
- Receptor informa qual espera

## 📌 Janela dinâmica
- Tamanho ajustado pelo receptor
- Baseado na capacidade de processamento
- Controle de fluxo eficiente

## 📌 Ataque SYN Flood
- Envia muitos SYN sem completar handshake
- Consome recursos do servidor
- Mitigação: SYN cookies