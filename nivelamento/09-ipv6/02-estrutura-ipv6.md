# Aula 2 – Estrutura do IPv6

## 📌 Formato
- 128 bits
- 8 grupos de 16 bits (hexadecatetos)
- Representação hexadecimal
- Separados por dois pontos (:)

## 📌 Exemplo
2001:0db8:85a3:0000:0000:8a2e:0370:7334

## 📌 Cada grupo (hexadecateto)
- 16 bits = 4 caracteres hexadecimais
- 0-9, A-F

## 📌 Comparação IPv4 x IPv6
| Característica | IPv4 | IPv6 |
|----------------|------|------|
| Bits | 32 | 128 |
| Formato | Decimal | Hexadecimal |
| Separador | . (ponto) | : (dois pontos) |
| Endereços | 4,3 bilhões | 340 undecilhões |
| Configuração | Manual/DHCP | SLAAC/DHCPv6 |

## 📌 Cabeçalho IPv6
- Mais simples que IPv4
- 8 campos fixos
- 40 bytes (tamanho fixo)
- Sem checksum (delega para camadas superiores)
- Suporte nativo a extensões