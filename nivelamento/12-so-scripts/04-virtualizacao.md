# Aula 4 – Virtualização

## 📌 O que é virtualização
- Simular hardware para rodar múltiplos sistemas
- Aproveitar melhor recursos de servidores
- Isolar ambientes

## 📌 Por que virtualizar
- Recursos subutilizados em servidores físicos
- Economia de energia e espaço
- Facilidade de gerenciamento
- Testes sem comprometer produção

## 📌 Hipervisor (Hypervisor)
- Software que gerencia máquinas virtuais

### Tipo 1 (Bare-metal)
- Roda diretamente no hardware
- Exemplos: Proxmox, VMware ESXi, Microsoft Hyper-V, XenServer
- Mais eficiente, usado em servidores

### Tipo 2 (Hosted)
- Roda sobre um sistema operacional
- Exemplos: VirtualBox, VMware Workstation
- Mais prático para testes e desktop

## 📌 Exemplo de alocação
Máquina física: CPU 8 núcleos, RAM 16GB, Disco 500GB

- VM1: 4 núcleos, 8GB RAM, 150GB
- VM2: 2 núcleos, 4GB RAM, 50GB
- VM3: 1 núcleo, 2GB RAM, 250GB

## 📌 Virtualização x Container
- **Virtualização:** virtualiza hardware
- **Container:** virtualiza sistema operacional (Docker, LXC)
- Containers são mais leves e rápidos

## 📌 Vantagens
- Menor consumo de energia
- Menos gasto com hardware
- Menos espaço em datacenters
- Isolamento e segurança