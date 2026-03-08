# Aula 5 – Conceitos básicos de banco de dados

## 📌 Introdução
- **Dados** → informações com significado (ex: nome, telefone)
- **Banco de dados** → conjunto organizado de dados armazenados

## 📌 Propriedades
- Organização, integridade, compartilhamento

## 📌 Tamanho e complexidade
- **Pequeno:** lista de contatos no celular
- **Grande:** Amazon (20M+ itens, 15M visitantes/dia)

## 📌 SGBD
- Sistema Gerenciador de Banco de Dados
- **Funções:** definir, construir, manipular, compartilhar

## 📌 Bancos Relacionais
- Organizam dados em tabelas com linhas e colunas
- Facilitam relacionamento entre conjuntos de dados
- **Exemplos:** MySQL, PostgreSQL, SQLite

## 📌 Chave Primária
- Campo que torna os dados únicos na tabela
- **Simples:** um único campo
- **Composta:** dois ou mais campos

## 📌 Relacionamentos
- Vínculo entre tabelas via chave estrangeira
- Chave estrangeira vincula à chave primária da tabela principal

## 📌 Bancos Não Relacionais (NoSQL)
- Grandes volumes de dados distribuídos
- Estruturas menos rígidas, dados não tabulares
- **Exemplos:** MongoDB (documentos), Cassandra, Redis (chave-valor)

## 📌 Bancos Distribuídos
- Espalhados fisicamente em múltiplos locais
- Alta disponibilidade e escalabilidade
- **Exemplos:** Cassandra, Couchbase

## 📌 Data Warehouses
- Otimizados para análise de grandes volumes
- Business intelligence, dados históricos
- **Exemplos:** Amazon Redshift, Google BigQuery

## 📌 SQL
- Structured Query Language
- **Criação:** `CREATE TABLE nome_tabela`
- **Consulta:** `SELECT * FROM nome_tabela`
- **Atualização:** `UPDATE tabela SET campo=valor`
- **Inserção:** `INSERT INTO tabela (campo1, campo2) VALUES (valor1, valor2)`