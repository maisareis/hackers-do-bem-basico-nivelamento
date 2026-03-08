# Aula 18 – Scripts Bash (Linux)

## 📌 O que é um script
- Arquivo de texto com comandos
- Interpretado pelo shell (bash)
- Automatiza tarefas repetitivas

## 📌 Estrutura básica
#!/bin/bash
# Comentário
comando1
comando2

## 📌 Variáveis
nome="João"
echo "Olá, $nome"

## 📌 Executando comandos
data=$(date)
echo "Hoje é $data"

## 📌 Exemplo: verificar portas abertas
#!/bin/bash
host="127.0.0.1"
for porta in 22 80 443; do
  nc -zv "$host" "$porta" 2>/dev/null && echo "Porta $porta aberta" || echo "Porta $porta fechada"
done

## 📌 Exemplo: monitorar log
#!/bin/bash
tail -f /var/log/auth.log | grep "Failed password"

## 📌 Exemplo: backup simples
#!/bin/bash
DATA=$(date +%Y%m%d)
tar -czf backup_$DATA.tar.gz /home/usuario/documentos
echo "Backup concluído: backup_$DATA.tar.gz"

## 📌 Condicionais
if [ "$nome" = "João" ]; then
  echo "É João"
else
  echo "Não é João"
fi

## 📌 Loops
for i in 1 2 3; do
  echo "Número $i"
done

while true; do
  echo "Loop infinito"
  sleep 1
done