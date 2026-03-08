# Aula 19 – Protocolo SSL/TLS

## 📌 SSL vs TLS
- SSL: Secure Sockets Layer (Netscape)
- TLS: Transport Layer Security (sucessor)

## 📌 Funcionamento
- Após three-way handshake do TCP
- Outro handshake inicia para criar canal seguro

## 📌 Processo simplificado
1. Usa criptografia assimétrica para criar canal seguro
2. Cria e transfere chave de criptografia simétrica
3. Melhor dos dois mundos: segurança da assimétrica + velocidade da simétrica

## 📌 Por que TLS substituiu SSL
- Protocolo importante não deveria pertencer a empresa privada
- Necessidade de versão não-proprietária
- Recorrentes problemas de segurança exigiam atualização constante

## 📌 Atualidade
- SSL está obsoleto
- Mais utilizado é TLS
- Nome SSL ficou popular, então SSL/TLS é usado como referência
- Tecnicamente, é TLS