# Aula 13 – Linux: File System

## 📌 EXT4 (Fourth Extended File System)
- Padrão no Linux
- Journaling (fsck para recuperação)
- Criptografia: sim
- Compactação: não
- Snapshots: não
- Limites: arquivo 16TB, partição 1EB

## 📌 Btrfs (B-Tree File System)
- Copy-on-Write (CoW)
- Autorreparo
- Criptografia, compactação, snapshots
- RAID, backup incremental, desduplicação
- Arquivo 16EB, partição 16EB

## 📌 XFS
- Alta performance (escalável)
- Journaling
- Aumentar tamanho online (não reduzir)
- Cotas
- Leitura/gravação paralela
- Arquivo 8EB, partição 16EB

## 📌 JFS (Journaled File System)
- Journaling
- Leve
- Arquivo 4PB, partição 32PB

## 📌 ReiserFS
- Journaling
- Bom para muitos arquivos pequenos
- Arquivo 8TB, partição 16TB

## 📌 ZFS
- Copy-on-Write, checksum, autorreparo
- Snapshots, RAID-Z, desduplicação
- Arquivo 16EB, partição 256 quadrilhões de ZB
- Original do Solaris, disponível no Linux

## 📌 Swap
- Memória virtual (disco)
- Usado quando RAM acaba
- Tamanho: múltiplo da RAM (2,4,8,16GB)