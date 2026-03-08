# Aula 1 – Tipos de ataques

## 📌 O que são Ataques Cibernéticos
- Esforço para roubar, expor, alterar, desativar ou destruir dados
- Acesso não autorizado a redes, sistemas ou dispositivos

## 📌 Principais tipos de ataque
- **Phishing** → mensagens falsas para enganar vítimas
- **Injection** → inserção de código malicioso (SQL, command, XSS)
- **Malware** → software malicioso (vírus, worm, trojan, ransomware)
- **Engenharia social** → manipulação psicológica
- **DDoS** → negação de serviço distribuída
- **Força bruta** → testar combinações de senha
- **MiTM** → interceptação de comunicação

## 📌 Engenharia Social e Phishing
- Phishing: se passar por entidades confiáveis
- **Spear phishing:** direcionado a alvos específicos
- **Whaling:** foco em executivos
- Identificar: erros gramaticais, URLs suspeitas

## 📌 Ataques Man-in-the-Middle (MiTM)
- Interceptar comunicações sem ser percebido
- Prevenção: HTTPS, VPN, verificação de certificados

## 📌 Força Bruta
- Testar todas combinações possíveis
- Ferramentas: hashcat com wordlists (ex: rockyou.txt)

## 📌 DoS e DDoS
- **DoS:** um único atacante
- **DDoS:** múltiplos dispositivos (botnet)
- Sobrecarregar serviços, tornando-os indisponíveis
- Ferramenta brasileira: T50 (testes de estresse)

## 📌 Injection
- SQL Injection, Command Injection
- Heartland Payment Systems (2008), Sony Pictures (2011)
- Prevenção: validação de entrada, consultas parametrizadas