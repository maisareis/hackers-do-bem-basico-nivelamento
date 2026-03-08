# Aula 17 – Linux: Gerenciamento de Pacotes

## 📌 Formas de instalação
1. Código-fonte (compilar)
2. Pacotes pré-compilados (.deb, .rpm)
3. Gerenciadores de pacotes
4. Gerenciadores universais (snap, flatpak)
5. AppImage

## 📌 Código-fonte
./configure
make
sudo make install

## 📌 Pacotes Debian/Ubuntu (.deb)
| Comando | Descrição |
|---------|-----------|
| `dpkg -i pacote.deb` | Instala .deb local |
| `dpkg -r pacote` | Remove |
| `dpkg -l` | Lista instalados |

## 📌 APT (Advanced Package Tool)
| Comando | Descrição |
|---------|-----------|
| `apt update` | Atualiza lista de pacotes |
| `apt upgrade` | Atualiza pacotes |
| `apt install pacote` | Instala |
| `apt remove pacote` | Remove |
| `apt search termo` | Busca |
| `apt show pacote` | Informações |

## 📌 Repositórios
- `/etc/apt/sources.list`
- Adicionar PPAs: `add-apt-repository ppa:nome`

## 📌 Pacotes Red Hat/Fedora (.rpm)
| Comando | Descrição |
|---------|-----------|
| `rpm -ivh pacote.rpm` | Instala |
| `rpm -e pacote` | Remove |
| `dnf install pacote` | Instala (Fedora) |
| `yum install pacote` | Instala (CentOS/RHEL) |

## 📌 Gerenciadores universais

### Snap
- Pacotes em sandbox
- `snap install pacote`
- `snap list`
- `snap remove pacote`

### Flatpak
- Similar ao snap
- `flatpak install pacote`
- `flatpak list`
- `flatpak remove pacote`

## 📌 AppImage
- Arquivo único, executável
- Baixar, dar permissão e executar
- `chmod +x aplicativo.AppImage`
- `./aplicativo.AppImage`
- Portátil (não instala no sistema)