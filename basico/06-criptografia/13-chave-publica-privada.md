# Aula 13 – Chave Pública e Privada (parte 1)

## 📌 O que são chaves digitais
- Códigos matematicamente relacionados
- Baseados em fatoração de números primos
- Matemática complexa (não abordada em detalhes)

## 📌 Cenário
- João quer mandar mensagem criptografada para Maria
- Não tem como garantir troca de chaves antes
- Decidem usar criptografia assimétrica

## 📌 Chaves envolvidas
- Chave Pública do João
- Chave Privada do João
- Chave Pública da Maria
- Chave Privada da Maria

## 📌 Processo
1. João criptografa mensagem com chave pública de Maria
2. Envia mensagem (como se colocasse cadeado)
3. Só chave privada de Maria pode abrir
4. Maria responde usando chave pública de João

## 📌 Segurança
- Mensagem trafega segura pela internet
- Mesmo interceptada, não conseguem ler
- Chave pública não consegue descriptografar o que ela mesma criptografou