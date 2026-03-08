# Aula 5 – Sub-redes

## 📌 O que é sub-rede
- Dividir uma rede em redes menores
- Emprestar bits da parte de host para rede
- Melhor aproveitamento de endereços

## 📌 Exemplo: dividir /24 em 2 sub-redes
Rede original: 192.168.0.0/24

Emprestar 1 bit da parte de host:
- Máscara nova: /25 (255.255.255.128)
- 2 sub-redes:
  - Sub-rede 1: 192.168.0.0/25
    - Primeiro IP: 192.168.0.1
    - Último IP: 192.168.0.126
    - Broadcast: 192.168.0.127
  - Sub-rede 2: 192.168.0.128/25
    - Primeiro IP: 192.168.0.129
    - Último IP: 192.168.0.254
    - Broadcast: 192.168.0.255

## 📌 Dividir /24 em 4 sub-redes
Emprestar 2 bits → /26 (255.255.255.192)
- Sub-rede 1: 192.168.0.0/26 (0-63)
- Sub-rede 2: 192.168.0.64/26 (64-127)
- Sub-rede 3: 192.168.0.128/26 (128-191)
- Sub-rede 4: 192.168.0.192/26 (192-255)

## 📌 Fórmulas
- Número de sub-redes = 2^(bits emprestados)
- Número de hosts por sub-rede = 2^(bits restantes) - 2