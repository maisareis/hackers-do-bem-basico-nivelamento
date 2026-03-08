# Aula 3 – Camada de Enlace

## 📌 Função
- Organizar os bits em quadros (frames)
- Controle de acesso ao meio
- Detecção de erros

## 📌 Divisão da camada (IEEE)
- **LLC** (Logical Link Control) - IEEE 802.2
- **MAC** (Media Access Control) - IEEE 802.3

## 📌 Endereçamento
- Endereço MAC (físico)
- 48 bits (6 bytes)
- Exemplo: B4:45:06:64:ED:9F

## 📌 Estrutura do quadro Ethernet
- **MAC destino** → 6 bytes
- **MAC origem** → 6 bytes
- **Tipo** → 2 bytes (ex: 0x0800 = IPv4)
- **Dados** → payload
- **FCS** → checksum para detecção de erros

## 📌 Dispositivos da camada 2
- **Switch** → encaminha baseado em MAC
- Ponte (bridge)
- Placa de rede (NIC)

## 📌 Tipos de comunicação
- **Unicast** → um para um
- **Broadcast** → um para todos (FF:FF:FF:FF:FF:FF)
- **Multicast** → um para grupo