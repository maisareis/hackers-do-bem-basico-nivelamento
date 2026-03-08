# Aula 4 – Endereço MAC

## 📌 O que é
- Media Access Control Address
- Endereço físico da placa de rede
- Gravado no hardware (ROM)

## 📌 Estrutura
- 48 bits (12 caracteres hexadecimais)
- **Primeiros 24 bits:** OUI (Organizationally Unique Identifier) → fabricante
- **Últimos 24 bits:** número de série do dispositivo

## 📌 Exemplo
B4:45:06:64:ED:9F
- B4:45:06 → Dell
- 64:ED:9F → número de série

## 📌 Como identificar fabricante
- Consultar bancos de dados OUI
- Sites como https://macvendors.com

## 📌 Tipos de endereço MAC
- **Unicast** → destinado a um único dispositivo
- **Broadcast** → para todos (FF:FF:FF:FF:FF:FF)

## 📌 Comandos úteis
- **Windows:** `ipconfig /all`
- **Linux:** `ip link` ou `ifconfig`
- **macOS:** `ifconfig`