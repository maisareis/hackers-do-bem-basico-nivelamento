# Aula 5 – Instalação de Sistemas Operacionais

## 📌 Preparação
- Criar mídia de instalação (DVD ou pendrive)
- Pendrive mínimo 8GB (preferência qualidade)
- Programas: Rufus, Ventoy, LinuxLive USB Creator

## 📌 Imagens ISO
- **Windows 10:** https://www.microsoft.com/pt-br/software-download/windows10
- **Ubuntu:** https://ubuntu.com/download/desktop
- **Proxmox:** https://www.proxmox.com/en/downloads

## 📌 Procedimento
1. Colocar pendrive no computador
2. Acessar BIOS/UEFI (Del, F2, F10, F12)
3. Alterar sequência de boot para pendrive
4. Salvar e reiniciar

## 📌 Instalação Windows
- Selecionar idioma/teclado
- "Não tenho chave do produto" (se aplicável)
- Escolher versão (Home, Pro, Education)
- Selecionar "Personalizada" (instalação limpa)
- Particionar disco (cuidado para não apagar errado)
- Aguardar cópia de arquivos
- Configurar região, usuário, senha

## 📌 Instalação Ubuntu
- "Try or Install Ubuntu"
- Selecionar idioma
- Escolher layout de teclado
- Tipo de instalação (normal ou mínima)
- Particionamento (automático ou manual)
  - / (root) → mínimo 15GB, recomendado 30-100GB
  - /boot/efi → 500MB-1GB
  - swap → múltiplo da RAM
  - /home → restante (opcional)
- Criar usuário e senha
- Escolher tema

## 📌 Instalação Proxmox
- "Install Proxmox VE (Graphical)"
- Aceitar EULA
- Selecionar país, timezone, teclado
- Configurar IP (estático recomendado)
- Definir senha e e-mail
- Aguardar instalação
- Acessar via navegador: https://IP:8006