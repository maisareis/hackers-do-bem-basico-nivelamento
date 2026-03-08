# Aula 7 – Controle de Usuários

## 📌 Evolução
- Primeiras redes: peer-to-peer, poucos computadores
- Crescimento das redes exigiu controle centralizado
- Surgimento dos serviços de diretório

## 📌 LDAP (Lightweight Directory Access Protocol)
- Protocolo para acesso a diretórios
- Versão leve do DAP
- Organização hierárquica em árvore
  - Diretório raiz
  - Países
  - Organizações
  - Unidades organizacionais
  - Indivíduos

## 📌 Active Directory (Microsoft)
- Serviço de diretório da Microsoft
- Baseado em LDAP
- Gerencia domínios, usuários, recursos
- Contém informações de todas as contas da rede

## 📌 Funcionamento
1. Usuário tenta conectar à rede
2. Requisição de autenticação ao servidor
3. Servidor consulta banco de dados
4. Resposta com acesso e permissões
5. Usuário acessa com privilégios definidos

## 📌 RADIUS (Remote Authentication Dial-In User Service)
- Protocolo AAA (Autenticação, Autorização, Contabilização)
- Desenvolvido em 1991
- Centraliza gerenciamento de acesso
- Usado em: wireless, VPN, servidores web
- Porta UDP 1812 (antiga 1645)

## 📌 Processo RADIUS
1. NAS consulta servidor RADIUS (Access-Request)
2. Servidor responde (Access-Accept ou Access-Reject)
3. Pode suportar múltiplos métodos de autenticação