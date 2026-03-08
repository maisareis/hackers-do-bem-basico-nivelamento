# Aula 15 – Função Hash

## 📌 Problema
- Conta que chega em casa: envelope violado?
- Programa baixado: foi modificado no caminho?
- Como verificar integridade no mundo digital?

## 📌 Definição
- Função matemática que recebe dados variados
- Sempre retorna quantidade fixa de caracteres

## 📌 Características
- Aceita dados de tamanho variável
- Produz valor de tamanho fixo
- 1 bit modificado na entrada → saída totalmente diferente
- Computacionalmente inviável reverter (descobrir mensagem original a partir do hash)

## 📌 Hash NÃO é criptografia
- Criptografia: reversível (com chave)
- Hash: processo unidirecional (não reversível)

## 📌 Importância do Hash
- Garante integridade da informação
- Mesma entrada → mesmo hash
- Entrada diferente → hash completamente diferente

## 📌 Aplicações
- Identificação de arquivos
- Validação de integridade
- Armazenamento de senhas

## 📌 Algoritmos
- MD5 (obsoleto, inseguro)
- SHA1 (obsoleto)
- SHA256, SHA512 (recomendados)