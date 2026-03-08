# Aula 7 – Windows: File System

## 📌 O que é sistema de arquivos
- Controla leitura e gravação no disco
- Gerencia localização das informações
- Controla permissões

## 📌 Como funciona
- **Gravação:**
  1. Divide o arquivo
  2. Atualiza tabela de arquivos
  3. Grava em vários lugares do disco

- **Leitura:**
  1. Pesquisa na tabela
  2. Pega todos pedaços
  3. Monta na RAM

## 📌 Setor x Cluster
- **Setor:** tamanho mínimo do fabricante (512 bytes)
- **Cluster:** tamanho definido na formatação (padrão 4KB)

## 📌 Tipos de sistema de arquivos Windows

### FAT32
- Usado no Windows 95 até ME
- Tamanho máximo disco: 32GB (Windows)
- Tamanho máximo arquivo: 4GB
- Atributos: somente leitura, oculto
- Sem permissões de segurança

### NTFS (New Technology File System)
- Padrão desde Windows XP
- Tamanho máximo: 8PB
- Permissões ACL (Access Control List)
- Atributos: criptografado, comprimido, offline
- Recursos: recuperação de dados, journaling, BitLocker

### ReFS (Resilient File System)
- Server 2012+, foco em dados
- Tamanho máximo: 35PB
- Verificação de integridade e autocorreção
- Desempenho para virtualização
- Snapshots
- Não inicializável (ainda)