# Aula 2 – Atores de ameaças

## 📌 O que são Atores de Ameaça
- Indivíduos, grupos ou entidades que representam ameaça
- Motivações e intenções variadas

## 📌 Tipos de Hackers
- **Black Hat** → maliciosos, agem ilegalmente
- **White Hat** → éticos, autorizados, melhoram segurança
- **Gray Hat** → entre os dois, sem autorização mas sem má intenção

## 📌 MITRE ATT&CK
- Base de conhecimento de táticas e técnicas adversárias
- Classifica grupos de ameaças por TTPs (Táticas, Técnicas e Procedimentos)
- Mapeia técnicas para mitigações
- https://attack.mitre.org/groups/

## 📌 APTs (Advanced Persistent Threats)
- Ataques complexos e sofisticados
- Realizados por atores estatais ou organizações criminosas bem financiadas
- Utilizam estrutura MITRE ATT&CK
- **Estágios:** Acesso inicial → Comando e Controle (C2) → Movimento lateral → Exfiltração

## 📌 Estudo de Caso: APT10 (Stone Panda)
- **Acesso inicial:** backdoor, credenciais roubadas
- **C2:** RAT RedLeaves
- **Movimento lateral:** Pass the Hash, Pass the Ticket
- **Exfiltração:** malware personalizado, serviços legítimos (Dropbox)

## 📌 Ameaças Internas
- Funcionários, contratados, parceiros com acesso privilegiado
- **Exemplo:** funcionário insatisfeito sabotando operações
- **Técnicas:** manipulação de contas, exfiltração
- Mitigação: monitoramento de comportamento anormal