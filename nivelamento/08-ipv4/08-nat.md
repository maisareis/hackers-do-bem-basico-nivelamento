# Aula 8 – NAT (Network Address Translation)

## 📌 O que é NAT
- Tradução de endereços de rede
- Converte IP privado em público e vice-versa
- Permite vários dispositivos compartilharem um único IP público

## 📌 Por que NAT
- IPv4 esgotado
- Vários dispositivos em casa/empresa
- Segurança (esconde rede interna)

## 📌 Funcionamento
1. Dispositivo (192.168.0.10) quer acessar Internet
2. Roteador recebe pacote
3. Roteador troca IP origem (privado) pelo IP público
4. Guarda tabela de tradução
5. Quando resposta volta, roteador reverte tradução

## 📌 Tipos de NAT
- **SNAT** (Source NAT) → traduz IP origem
- **DNAT** (Destination NAT) → traduz IP destino (port forwarding)
- **PAT** (Port Address Translation) → traduz portas também

## 📌 Exemplo prático
- Rede interna: 192.168.0.0/24
- Roteador: IP público 200.100.50.1
- Todos dispositivos saem com IP 200.100.50.1
- Roteador diferencia por porta de origem

## 📌 Limitações
- Dificulta conexões entrantes
- Precisa de port forwarding para servidores internos
- Não é necessário no IPv6