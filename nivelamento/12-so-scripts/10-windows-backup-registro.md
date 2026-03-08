# Aula 9 – Windows: Usuários e Permissões

## 📌 Criação de usuários

### Modo gráfico
- **Gerenciamento do computador** → Usuários e grupos locais (Windows Pro+)
- **Configurações** → Contas → Família e outros usuários (Windows Home)
- **control userpasswords2** → gerencia senhas

### Linha de comando
net user nome senha /add
net user nome /del
net localgroup Administradores nome /add

## 📌 Tipos de usuários
- **Administrador:** controle total, pode instalar programas, alterar configurações
- **Usuário padrão:** limitado, não instala programas sem elevação

## 📌 Permissões NTFS

| Permissão | Arquivo | Pasta |
|-----------|---------|-------|
| **Listar** | - | Visualiza conteúdo |
| **Ler** | Ver arquivo | Acessar pasta |
| **Ler e executar** | Ver e executar | Acessar e percorrer |
| **Escrever** | Editar | Criar subpastas |
| **Modificar** | Ler, escrever, executar | Ler, criar, modificar |
| **Controle total** | Tudo | Tudo |

## 📌 Compartilhamento de rede
- Apenas administrador pode compartilhar
- Usuário sem senha não acessa compartilhamento
- Se nome/senha iguais em ambos PCs, acesso direto
- Senão, pede credenciais
- Limite Windows 10: 20 conexões simultâneas