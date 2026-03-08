# Aula 16 – Ataques em Hashes

## 📌 Como o computador armazena senhas
- Não armazena a senha em texto claro
- Armazena o HASH da senha

## 📌 Fraqueza do hash puro
- Sempre a mesma entrada → mesmo hash
- Permite ataque de rainbow table
- Se duas pessoas têm mesmo hash, têm mesma senha

## 📌 Rainbow Table
- Tabela pré-computada de hashes
- Compara hashes roubados com a tabela
- Descobre senhas por correspondência

## 📌 Solução: Salt
- "Código" extra misturado à senha antes do hash
- Mesma senha com salts diferentes → hashes diferentes
- Torna rainbow table inútil

## 📌 Como sistemas modernos armazenam senhas
- Hash + salt
- Impossível usar rainbow table
- Segurança muito maior

## 📌 Conclusão
- Importante entender fraquezas dos hashes
- Saber como se proteger
- Base para certificados digitais (próxima aula)