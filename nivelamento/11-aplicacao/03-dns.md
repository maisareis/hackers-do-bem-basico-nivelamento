# Aula 3 – DNS (Domain Name System)

## 📌 O que é DNS
- Sistema de Nomes de Domínio
- Converte nomes (google.com) em endereços IP
- "Lista telefônica da internet"
- Criado em 1983 por Paul Mockapetris

## 📌 Por que precisa
- Humanos memorizam nomes
- Computadores usam números (IP)
- DNS faz a tradução

## 📌 Servidores DNS
1. **Recursor DNS** → recebe consulta do cliente
2. **Servidor Raiz** → direciona para TLD
3. **Nameserver TLD** → direciona para autoritativo (.com, .org)
4. **Servidor Autoritativo** → tem a resposta final

## 📌 Processo de resolução

Cliente → Recursor → Servidor Raiz → Servidor TLD → Servidor Autoritativo → Resposta

## 📌 Cache DNS
- Armazenamento temporário de respostas
- Aumenta desempenho
- Reduz tráfego
- Diminui latência

## 📌 Tipos de registro
- **A** → IPv4
- **AAAA** → IPv6
- **CNAME** → alias (apelido)
- **MX** → servidor de e-mail
- **NS** → servidor DNS
- **TXT** → texto (verificações, SPF)