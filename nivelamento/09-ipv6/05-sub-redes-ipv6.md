# Aula 5 – Sub-redes IPv6

## 📌 Prefixo padrão /64
- 64 bits para rede
- 64 bits para interface (host)
- 2^64 hosts por sub-rede

## 📌 Estrutura
2001:f0f0:dad0:cafe:0005:0006:0007:0008 /64

- **Rede:** 2001:f0f0:dad0:cafe
- **Host:** 0005:0006:0007:0008

## 📌 Próxima rede
Rede atual: 2001:f0f0:dad0:cafe::/64

Próxima rede: 2001:f0f0:dad0:caff::/64

## 📌 Dividindo em sub-redes
Emprestar bits da parte de host

### /65 (emprestar 1 bit)
- Sub-rede 1: 2001:f0f0:dad0:cafe:0000::/65 (0000 - 7fff)
- Sub-rede 2: 2001:f0f0:dad0:cafe:8000::/65 (8000 - ffff)

### /66 (emprestar 2 bits)
- Sub-redes: 0000, 4000, 8000, c000 (avança 4 em 4)

### /67 (emprestar 3 bits)
- Sub-redes: 0000, 2000, 4000, 6000, 8000, a000, c000, e000 (avança 2 em 2)

## 📌 Fórmula
- Número de sub-redes = 2^(bits emprestados)
- Espaço entre sub-redes = 2^(16 - bits emprestados) em hexadecimal