# Aula 5 – OWASP Top 10 (parte 2)

## 📌 A06:2021 – Vulnerable and Outdated Components (Componentes Vulneráveis)
- Uso de bibliotecas, frameworks com falhas conhecidas
- Versões desatualizadas sem patches de segurança
- Facilita exploração por ataques conhecidos

## 📌 A07:2021 – Identification and Authentication Failures (Falhas de Identificação e Autenticação)
- Falhas em mecanismos de autenticação
- Senhas fracas, credenciais padrão
- Falta de proteção contra força bruta

## 📌 A08:2021 – Software and Data Integrity Failures (Falhas de Integridade)
- Atualizações sem verificação de integridade
- Dependências não verificadas
- CI/CD sem validação de segurança

## 📌 A09:2021 – Security Logging and Monitoring Failures (Falhas de Registro e Monitoramento)
- Ausência de logs de segurança
- Incapacidade de detectar incidentes
- Falta de alertas em tempo real

## 📌 A10:2021 – Server-Side Request Forgery (SSRF)
- Aplicação faz requisições não autorizadas a outros servidores
- Expõe informações internas
- Permite ataques a sistemas internos