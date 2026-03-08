# Aula 3 – APTs (Ameaças Persistentes Avançadas)

## 📌 Definição
- Ataques cibernéticos complexos e sofisticados
- Realizados por atores estatais ou organizações criminosas
- Utilizam estrutura MITRE ATT&CK

## 📌 Estágios de uma APT
1. **Acesso Inicial**
   - Exploração de vulnerabilidades
   - Ataques de senha (força bruta, pulverização)
   - Comprometimento de software de terceiros

2. **Comando e Controle (C2)**
   - Estabelecer canal de comunicação
   - Instalação de RATs (Remote Access Trojans)
   - Uso de DGAs (Domain Generation Algorithms)

3. **Movimento Lateral**
   - Pass-the-Hash
   - Exploração de serviços mal configurados
   - Roubo de credenciais (Mimikatz)

4. **Exfiltração de Dados**
   - Esteganografia
   - Criptografia
   - Uso de canais C2

## 📌 Estudo de Caso: APT10 (Stone Panda)
- **RedLeaves:** RAT para C2
- **Pass the Ticket:** burlar autenticação no Active Directory
- **Dropbox:** disfarçar tráfego malicioso

## 📌 Mitigação
- Conscientização de segurança
- Atualização e patch de sistemas
- Defesa em profundidade
- Colaboração e compartilhamento de informações