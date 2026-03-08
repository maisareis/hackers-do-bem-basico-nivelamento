# Aula 4 – Abreviações IPv6

## 📌 Regra 1: Remover zeros à esquerda
2001:0db8:00c0:00a5:0000:0000:0000:1234

Remove zeros à esquerda:
2001:db8:c0:a5:0:0:0:1234

## 📌 Regra 2: Dois pontos duplos (::)
- Substitui sequências contínuas de zeros
- Só pode usar uma vez no endereço

2001:db8:c0:a5:0:0:0:1234 → 2001:db8:c0:a5::1234

## 📌 Exemplos
Endereço completo:
2001:0000:0000:0000:0000:0000:0000:0001

Abreviado:
2001::1

Endereço completo:
2001:0db8:0000:0000:0000:0000:0000:0002

Abreviado:
2001:db8::2

## 📌 Exercícios
- 2001:cafe:0000:0000:0000:0000:0000:0099 → 2001:cafe::99
- 2001:f0f0:dad0:cafe:0005:0006:0007:0008 → 2001:f0f0:dad0:cafe:5:6:7:8
- 2001:0000:0000:cafe:0000:0000:0000:0001 → 2001::cafe:0:0:0:1 (cuidado: só um ::)