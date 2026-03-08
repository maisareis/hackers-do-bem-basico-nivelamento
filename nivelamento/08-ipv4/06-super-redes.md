# Aula 6 – Super-redes

## 📌 O que é super-rede
- Juntar várias redes menores em uma rede maior
- Útil quando empresa precisa de mais endereços
- Também chamado de agregação ou CIDR

## 📌 Exemplo
Redes: 192.168.0.0/24 e 192.168.1.0/24
- Juntar em: 192.168.0.0/23

Máscara: 255.255.254.0
- 2 redes /24 = 510 hosts (512 - 2)

## 📌 Cuidados
- 192.168.1.0/23 **não é** endereço de rede
- O endereço de rede é 192.168.0.0/23
- 192.168.1.0 é um IP válido dentro da super-rede

## 📌 Outro exemplo
Redes: 192.168.2.0/24 e 192.168.3.0/24
- Juntar em: 192.168.2.0/23
- 510 IPs válidos

## 📌 Benefícios
- Reduz tabelas de roteamento
- Melhor aproveitamento de endereços
- Simplifica gerenciamento