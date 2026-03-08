# Aula 5 – Cifra de Vigenère

## 📌 Funcionamento
- Utiliza Quadro de Vigenère
- Define uma chave (palavra ou frase)

## 📌 Exemplo
Mensagem: O ataque irá ocorrer as dez horas
Chave: HACKERS DO BEM

**Processo:**
1. Tirar espaços e alinhar mensagem com chave

OATAQUEIRAOCORRERASDEZHORAS
HACKERSDOBEMHACKERSDOBEMHAC

2. Cruzar letra da mensagem com letra da chave no quadro
3. Resultado: V avkulw lfb sovrtov rk gsa layau

## 📌 Descriptografar
- Precisa da chave
- Coluna = letra da chave
- Encontrar letra cifrada na coluna
- Linha correspondente = letra original

## 📌 Força da Cifra
- Muito forte por séculos
- Mesma letra pode ser cifrada de várias formas
- Resistente à análise de frequência