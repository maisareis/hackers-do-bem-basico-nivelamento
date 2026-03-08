# Aula 14 – Linux: Navegação e Comandos

## 📌 Ubuntu Desktop
- Área de trabalho (ícones, papel de parede)
- Botão Atividades (visão geral, busca)
- Dock (barra de aplicativos)
- Calendário no painel superior

## 📌 Navegação básica
| Comando | Descrição |
|---------|-----------|
| `ls` | Lista arquivos |
| `ls -la` | Lista tudo (inclusive ocultos, permissões) |
| `cd /caminho` | Muda diretório |
| `cd ..` | Volta um nível |
| `pwd` | Mostra caminho atual |
| `mkdir nome` | Cria pasta |
| `rm nome` | Remove arquivo |
| `rm -rf pasta` | Remove pasta (cuidado!) |
| `cp origem destino` | Copia |
| `cp -r origem destino` | Copia pasta |
| `mv origem destino` | Move/renomeia |
| `cat arquivo` | Mostra conteúdo |
| `nano arquivo` | Edita texto |
| `touch arquivo` | Cria arquivo vazio |

## 📌 Permissões
| Comando | Descrição |
|---------|-----------|
| `chmod 755 arquivo` | Muda permissão (dono=rwx, grupo=r-x, outros=r-x) |
| `chmod u+x arquivo` | Adiciona execução |
| `chown usuario:grupo arquivo` | Muda dono e grupo |
| `chgrp grupo arquivo` | Muda apenas grupo |

## 📌 Processos e sistema
| Comando | Descrição |
|---------|-----------|
| `ps aux` | Lista processos |
| `top` | Monitora processos |
| `htop` | Top melhorado |
| `kill PID` | Mata processo |
| `df -h` | Espaço em disco |
| `du -sh pasta` | Tamanho da pasta |
| `free -h` | Memória RAM |
| `uname -a` | Info do sistema |