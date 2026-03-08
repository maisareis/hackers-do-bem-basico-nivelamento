# Aula 6 – Protocolo ARP

## 📌 O que é ARP
- Address Resolution Protocol
- Resolve endereço IP → endereço MAC

## 📌 Por que precisa
- Camada 3 (IP) precisa saber MAC da camada 2
- Para montar o quadro Ethernet

## 📌 Funcionamento
1. Dispositivo A quer falar com IP 10.0.0.1
2. Verifica na tabela ARP se já tem MAC
3. Se não tem, envia **ARP Request** (broadcast)
   - "Quem tem o IP 10.0.0.1?"
4. Dispositivo com IP 10.0.0.1 responde **ARP Reply** (unicast)
   - "10.0.0.1 está em 00:D7:6D:68:91:07"
5. Dispositivo A guarda na tabela ARP

## 📌 Tabela ARP
- Cache com pares IP → MAC
- Entradas expiram após algum tempo

## 📌 Comandos úteis
- **Windows:** `arp -a`
- **Linux:** `arp -n` ou `ip neigh`

## 📌 ARP Spoofing (ataque)
- Atacante envia ARP Reply falso
- Associa IP legítimo ao MAC do atacante
- Tráfego é redirecionado (MITM)