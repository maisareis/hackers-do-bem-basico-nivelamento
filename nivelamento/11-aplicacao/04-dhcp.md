# Aula 4 – DHCP (Dynamic Host Configuration Protocol)

## 📌 O que é DHCP
- Protocolo de configuração dinâmica de host
- Atribui configurações IP automaticamente
- Evolução do BOOTP

## 📌 Por que usar
- Elimina configuração manual
- Evita conflitos de IP
- Ideal para grandes redes
- Dispositivos móveis (plug-and-play)

## 📌 Processo DORA

**D**iscover (Cliente → Servidor)
- Cliente envia broadcast procurando servidor DHCP

**O**ffer (Servidor → Cliente)
- Servidor oferece um IP e configurações

**R**equest (Cliente → Servidor)
- Cliente aceita a oferta

**A**cknowledge (Servidor → Cliente)
- Servidor confirma e finaliza

## 📌 Informações fornecidas
- Endereço IP
- Máscara de rede
- Gateway padrão (roteador)
- Servidores DNS
- Tempo de concessão (lease)

## 📌 Portas
- Servidor: UDP 67
- Cliente: UDP 68