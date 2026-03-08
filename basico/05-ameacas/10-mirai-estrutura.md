# Aula 10 – Mirai: Estrutura e Comunicação

## 📌 Arquitetura do Código
- **Servidor C&C/C2:** escrito em Go
- **Bots:** escritos em C (otimizados para IoT)

## 📌 Componentes principais

### attack.go
- Define ataques disponíveis (UDP flood, SYN flood, etc.)
- Mapeia flags de configuração (tamanho do pacote, duração)

### scanner.c
- Gerencia conexões para brute force
- Busca prompts de login ("assword")
- Controla máquina de estados da conexão

### killer.c
- Mata processos que usam portas específicas
- Evita concorrência de outros malwares
- Verifica /proc/net/tcp periodicamente

## 📌 Comunicação Bots x C2
- Dispositivos infectados registram-se no botnet
- Estabelecem comunicação com C2
- Recebem instruções (ataques DDoS, propagação)
- Comunicação projetada para ser anônima

## 📌 Registro na Botnet
- Primeiro passo após infecção
- Comunicação com servidor C2
- Dispositivo integrado à rede
- Pronto para receber comandos

## 📌 Segurança e Anonimato
- Criptografia nas comunicações
- Técnicas para ocultar origem dos ataques
- Proteção contra análise por pesquisadores