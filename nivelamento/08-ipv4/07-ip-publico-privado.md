# Aula 7 – IP Público e Privado

## 📌 IP Público
- Globalmente único na Internet
- Atribuído por provedores (ISP)
- Precisa ser roteável na Internet
- Controlado por IANA e RIRs (LACNIC, ARIN, etc.)

## 📌 IP Privado
- Usado em redes locais (LAN)
- Pode ser repetido em redes diferentes
- Não roteável na Internet
- Definido pela RFC 1918

## 📌 Faixas de IP Privado (RFC 1918)

| Classe | Rede | Máscara | Faixa |
|--------|------|---------|-------|
| A | 10.0.0.0 | /8 | 10.0.0.0 - 10.255.255.255 |
| B | 172.16.0.0 | /12 | 172.16.0.0 - 172.31.255.255 |
| C | 192.168.0.0 | /16 | 192.168.0.0 - 192.168.255.255 |

## 📌 Comparativo

| Característica | IP Privado | IP Público |
|----------------|------------|------------|
| Uso | LAN | WAN/Internet |
| Único? | Não, pode repetir | Sim, globalmente único |
| Atribuição | Adm. local | ISP/IANA |
| Custo | Gratuito | Pago |
| Esgotamento | Não se esgota | Esgotado |