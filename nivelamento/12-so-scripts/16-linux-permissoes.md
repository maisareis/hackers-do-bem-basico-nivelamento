# Aula 16 – Linux: Permissões

## 📌 Tipos de permissão
- **r (read)** → leitura
- **w (write)** → escrita
- **x (execute)** → execução

## 📌 Níveis de permissão
- **u (user)** → dono do arquivo
- **g (group)** → grupo do arquivo
- **o (others)** → outros usuários
- **a (all)** → todos (u+g+o)

## 📌 Visualizando permissões
`ls -l`

Exemplo: `-rwxr-xr--`

- **Primeiro caractere:** `-` (arquivo), `d` (diretório), `l` (link)
- **2-4:** permissões do dono (rwx)
- **5-7:** permissões do grupo (r-x)
- **8-10:** permissões de outros (r--)

## 📌 Notação octal

| Número | Binário | Permissão |
|--------|---------|-----------|
| 0 | 000 | --- |
| 1 | 001 | --x |
| 2 | 010 | -w- |
| 3 | 011 | -wx |
| 4 | 100 | r-- |
| 5 | 101 | r-x |
| 6 | 110 | rw- |
| 7 | 111 | rwx |

## 📌 Exemplos
- `chmod 755 arquivo` → dono rwx, grupo r-x, outros r-x
- `chmod 644 arquivo` → dono rw-, grupo r--, outros r--
- `chmod 700 pasta` → dono rwx, grupo ---, outros ---

## 📌 Modo simbólico
- `chmod u+x arquivo` → adiciona execução para dono
- `chmod g-w arquivo` → remove escrita do grupo
- `chmod o=r arquivo` → define outros como leitura

## 📌 Permissões em diretórios
- **r:** lista conteúdo (ls)
- **w:** cria/remove arquivos
- **x:** acessa diretório (cd)

## 📌 Exemplos práticos
- **500 (r-x--x--x):** acessa e lista, mas não modifica
- **700 (rwx------):** só dono tem tudo
- **000 (---------):** só root acessa