# Aula 15 – Linux: Usuários e Grupos

## 📌 Arquivos de configuração
- `/etc/passwd` → lista de usuários (nome, UID, diretório)
- `/etc/shadow` → senhas criptografadas
- `/etc/group` → grupos

## 📌 Comandos para usuários
| Comando | Descrição |
|---------|-----------|
| `whoami` | Usuário atual |
| `sudo comando` | Executa como root |
| `su -` | Vira root |
| `useradd -m nome` | Cria usuário com home |
| `adduser nome` | Cria usuário (amigável) |
| `passwd nome` | Altera senha |
| `userdel nome` | Remove usuário |
| `usermod -aG grupo usuario` | Adiciona a grupo |

## 📌 Comandos para grupos
| Comando | Descrição |
|---------|-----------|
| `groupadd nome` | Cria grupo |
| `groupdel nome` | Remove grupo |
| `groups usuario` | Mostra grupos do usuário |

## 📌 Tipos de usuários
- **Root (UID 0):** superusuário, controle total
- **Sistema (UID 1-999):** serviços (apache, mysql)
- **Humanos (UID 1000+):** usuários comuns

## 📌 Exemplo
sudo adduser aluno
sudo passwd aluno
sudo usermod -aG sudo aluno

- `adduser` cria usuário, home, grupo, pede senha
- `passwd` altera/define senha
- `usermod -aG sudo` adiciona ao grupo sudo (pode usar sudo)