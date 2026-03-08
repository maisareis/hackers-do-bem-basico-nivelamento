# Aula 3 – Tipos de Endereço IPv6

## 📌 Tipos de comunicação
- **Unicast** → um para um
- **Multicast** → um para grupo
- **Anycast** → um para o mais próximo (novo no IPv6)
- **Broadcast** → não existe no IPv6 (usar multicast)

## 📌 Categorias de endereço

### Global Unicast (2000::/3)
- Equivalente ao IPv4 público
- Roteável na Internet
- Atribuído por provedores

### Unique Local (FC00::/7)
- Equivalente ao IPv4 privado
- Não roteável na Internet
- Para redes internas

### Link Local (FE80::/10)
- Comunicação no mesmo enlace/rede
- Atribuído automaticamente
- Não roteável

### Loopback (::1)
- Equivalente a 127.0.0.1
- Próprio dispositivo

## 📌 Multicast (FF00::/8)
- Comunicação para grupos
- Exemplo: FF02::1 (todos os nós na rede local)
- Exemplo: FF02::2 (todos os roteadores)