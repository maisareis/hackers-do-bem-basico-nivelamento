# Aula 8 – Gerenciamento e Monitoramento

## 📌 Surgimento
- Décadas de 1960-1970
- Protocolos específicos para gerenciamento
- Papel estratégico em TI

## 📌 SNMP (Simple Network Management Protocol)
- Coleta, organiza e envia dados de dispositivos de rede
- 3 versões (V3 é a mais atual, com segurança)
- Porta UDP 161

### Funções do SNMP
- Monitoramento de desempenho
- Detecção e resolução de problemas
- Configuração de dispositivos
- Notificação de eventos (traps)

## 📌 SYSLOG
- Protocolo de logging do sistema
- Armazena mensagens de eventos
- Porta UDP 514

### Funções do SYSLOG
- Monitoramento
- Solução de problemas
- Segurança (auditoria)
- Conformidade
- Análise e planejamento

### Funcionamento
1. Dispositivo gera evento
2. Envia mensagem para servidor SYSLOG
3. Servidor armazena e analisa

## 📌 NTP (Network Time Protocol)
- Sincronização de horário
- Porta UDP 123
- Fundamental para logs e auditoria
- Hierarquia de servidores (stratum)

## 📌 Importância
- Visibilidade da rede
- Identificação proativa de problemas
- Base para análise forense
- Suporte a conformidade (LGPD, PCI DSS)