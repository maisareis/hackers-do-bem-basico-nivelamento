# Aula 6 – Cabeçalho IPv6

## 📌 Comparação com IPv4
- IPv4: 12 campos fixos, 20-60 bytes
- IPv6: 8 campos fixos, 40 bytes

## 📌 Cabeçalho IPv6

| Campo | Tamanho | Função |
|-------|---------|--------|
| Versão | 4 bits | 6 (IPv6) |
| Classe de tráfego | 8 bits | QoS, prioridade |
| Identificador de fluxo | 20 bits | Identifica fluxos especiais |
| Tamanho dos dados | 16 bits | Tamanho do payload |
| Próximo cabeçalho | 8 bits | Tipo do próximo cabeçalho (TCP, UDP, extensão) |
| Limite de encaminhamento | 8 bits | Equivalente ao TTL |
| Endereço de origem | 128 bits | IP de origem |
| Endereço de destino | 128 bits | IP de destino |

## 📌 Vantagens
- Mais simples
- Mais rápido de processar
- Roteadores intermediários não processam cabeçalhos de extensão
- Sem checksum (delega para camadas superiores)
- Suporte nativo a jumbograms (pacotes maiores)

## 📌 Cabeçalhos de extensão
- Fragmentação
- Autenticação (AH)
- Segurança (ESP)
- Roteamento
- Opções de destino/hop