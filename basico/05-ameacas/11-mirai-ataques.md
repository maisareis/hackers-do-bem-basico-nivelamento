# Aula 11 – Mirai: Técnicas de Ataque

## 📌 Funções de ataque
- **attack_udp_generic:** UDP flood genérico
- **attack_udp_vse:** UDP amplificado (Valve Source Engine)
- **attack_udp_dns:** Ataque a servidores DNS
- **attack_tcp_syn:** TCP SYN flood
- **attack_tcp_stomp:** TCP STOMP

## 📌 Processo de ataque
1. Usuário autentica na API
2. Comando de ataque é processado
3. Alvos são parseados (prefixo/máscara)
4. Comando é enfileirado para os bots

## 📌 Distribuição do ataque
- Dispositivos infectados recebem comando
- Geram tráfego massivo simultaneamente
- Cooperação entre bots para sobrecarregar alvo
- Cada bot contribui para o volume total

## 📌 Impactos
- Sobrecarga de redes e servidores
- Comprometimento de dispositivos IoT
- Interferência em serviços críticos
- Amplificação dos ataques
- Custo financeiro para mitigação e recuperação

## 📌 Por que estudar Mirai
- Aprendizado em C e Go
- Protocolos de rede (TCP/IP)
- Vulnerabilidades de IoT
- Funcionamento de botnets e ataques DDoS