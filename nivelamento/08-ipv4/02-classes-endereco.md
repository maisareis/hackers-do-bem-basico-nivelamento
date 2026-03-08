# Aula 2 – Classes de Endereço IPv4

## 📌 Sistema Classful
- Divisão do espaço IPv4 em classes
- Baseado nos primeiros bits do endereço

## 📌 Classes

| Classe | Início | Fim | Máscara padrão | Bits iniciais |
|--------|--------|-----|----------------|---------------|
| A | 1.0.0.0 | 126.255.255.255 | 255.0.0.0 (/8) | 0 |
| B | 128.0.0.0 | 191.255.255.255 | 255.255.0.0 (/16) | 10 |
| C | 192.0.0.0 | 223.255.255.255 | 255.255.255.0 (/24) | 110 |
| D | 224.0.0.0 | 239.255.255.255 | Multicast | 1110 |
| E | 240.0.0.0 | 255.255.255.255 | Reservado | 1111 |

## 📌 Observações
- Classe A: redes grandes (16 milhões de hosts)
- Classe B: redes médias (65 mil hosts)
- Classe C: redes pequenas (254 hosts)
- Classe D: multicast (não divide em rede/host)
- Classe E: experimental/reservado

## 📌 Exceção
- 127.0.0.0/8 → loopback (próprio dispositivo)