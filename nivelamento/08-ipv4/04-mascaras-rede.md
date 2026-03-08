# Aula 4 – Máscaras de Rede

## 📌 O que é máscara de rede
- Divide o IP em duas partes:
  - **Rede** → bits fixos (1 na máscara)
  - **Host** → bits variáveis (0 na máscara)

## 📌 Exemplo
IP: 192.168.1.100
Máscara: 255.255.255.0

Binário:
IP:       11000000.10101000.00000001.01100100
Máscara:  11111111.11111111.11111111.00000000
Rede:     11000000.10101000.00000001.00000000 → 192.168.1.0
Host:     00000000.00000000.00000000.01100100 → 100

## 📌 Endereços especiais
- **Endereço de rede:** todos bits de host = 0 (ex: 192.168.1.0)
- **Endereço de broadcast:** todos bits de host = 1 (ex: 192.168.1.255)
- **Endereços válidos:** entre rede e broadcast (ex: 192.168.1.1 a 192.168.1.254)

## 📌 Cálculo de hosts
- Número de hosts = 2^(bits de host) - 2
- Subtrai 2 (rede e broadcast)

## 📌 Exemplos
- /24 (255.255.255.0) → 2^8 - 2 = 254 hosts
- /16 (255.255.0.0) → 2^16 - 2 = 65.534 hosts
- /8 (255.0.0.0) → 2^24 - 2 = 16.777.214 hosts