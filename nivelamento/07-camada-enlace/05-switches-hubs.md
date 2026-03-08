# Aula 5 – Switches e Hubs

## 📌 Hub (camada 1)
- Repetidor de sinais elétricos
- Envia quadro para **todas as portas**
- Gera tráfego desnecessário
- Dispositivo obsoleto

## 📌 Switch (camada 2)
- Encaminha quadro apenas para a porta de destino
- Baseado em tabela MAC
- Aprende endereços automaticamente
- Mais eficiente que hub

## 📌 Tabela MAC
- Mapeia endereço MAC → porta
- Construída dinamicamente
- Switches aprendem conforme recebem quadros

## 📌 Funcionamento
1. Switch recebe quadro
2. Verifica MAC destino na tabela
3. Se encontrado → encaminha só para aquela porta
4. Se não encontrado → envia para todas (flood)

## 📌 Vantagens do switch
- Reduz colisões
- Melhora performance
- Segmenta tráfego
- Mais seguro que hub