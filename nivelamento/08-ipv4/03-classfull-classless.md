# Aula 3 – Classfull x Classless

## 📌 Classfull
- Roteamento baseado em classes A, B, C
- Máscara fixa pela classe
- Desperdício de endereços
- Exemplo: empresa com 300 hosts
  - Classe B (65 mil hosts) → muito grande
  - Classe C (254 hosts) → insuficiente

## 📌 Classless (CIDR)
- Classless Inter-Domain Routing
- RFC 1519 (1993)
- Máscara de tamanho variável (VLSM)
- Notação: IP/máscara (ex: 192.168.1.0/24)

## 📌 Vantagens
- Aproveitamento melhor dos endereços
- Agregação de rotas (super-redes)
- Mais flexibilidade

## 📌 Notação CIDR
| Máscara | CIDR | Hosts |
|---------|------|-------|
| 255.0.0.0 | /8 | 16.777.214 |
| 255.255.0.0 | /16 | 65.534 |
| 255.255.255.0 | /24 | 254 |
| 255.255.255.128 | /25 | 126 |
| 255.255.255.192 | /26 | 62 |
| 255.255.255.224 | /27 | 30 |
| 255.255.255.240 | /28 | 14 |
| 255.255.255.248 | /29 | 6 |
| 255.255.255.252 | /30 | 2 |