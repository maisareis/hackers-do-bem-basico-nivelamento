# Aula 9 – Mirai: Infecção e Propagação

## 📌 O que é Mirai
- Botnet que ataca dispositivos IoT
- Código aberto (estudo didático)
- Escrito em C (bots) e Go (servidor C2)

## 📌 Scanner do Mirai
- Testa combinações de usuário/senha padrão
- Credenciais comuns: root/xc3511, root/vizxv, root/admin, admin/admin

## 📌 Processo de Infecção
1. Scanner envia pacotes SYN para IPs aleatórios (porta 23/Telnet)
2. Se recebe SYN-ACK, dispositivo está vivo
3. Tenta brute force com combinações de credenciais
4. Se autentica, reporta ao controlador

## 📌 Estabelecimento C2
- Dispositivo resolve domínio do C2
- Estabelece comunicação
- Recebe comandos (attack_parse)

## 📌 Propagação
- Após infectar, busca novos alvos automaticamente
- Recebe instruções do C2
- Natureza autossustentável
- Gera IPs aleatórios continuamente

## 📌 Técnica de Brute Force
- Explora segurança frágil de dispositivos IoT
- Credenciais padrão não alteradas
- Necessidade de trocar senhas padrão
- Grande quantidade de dispositivos vulneráveis