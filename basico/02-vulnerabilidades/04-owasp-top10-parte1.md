# Aula 4 – OWASP Top 10 (parte 1)

## 📌 OWASP
- Open Web Application Security Project
- Organização internacional sem fins lucrativos
- Foco em segurança de aplicativos web
- Publica o Top 10 das vulnerabilidades mais críticas

## 📌 A01:2021 – Broken Access Control (Controle de Acesso Quebrado)
- Usuários não autorizados acessam recursos restritos
- Resulta em violações de privacidade, vazamento de informações
- Exemplo: acessar URL direta sem permissão

## 📌 A02:2021 – Cryptographic Failures (Falhas Criptográficas)
- Uso inadequado de criptografia
- Dados sensíveis expostos
- Exemplo: senhas armazenadas sem hash, tráfego sem TLS

## 📌 A03:2021 – Injection (Injeção)
- Dados não confiáveis são tratados como código
- **SQL Injection** → comandos SQL maliciosos
- **Command Injection** → comandos do sistema
- **Cross-Site Scripting (XSS)** → scripts maliciosos no navegador

## 📌 A04:2021 – Insecure Design (Design Inseguro)
- Falhas no projeto da aplicação
- Ausência de práticas de segurança desde o início
- Exemplo: não definir limites de taxa em APIs

## 📌 A05:2021 – Security Misconfiguration (Configuração Incorreta)
- Configurações padrão não alteradas
- Serviços desnecessários ativos
- Mensagens de erro detalhadas expondo informações