# Aula 19 – Scripts PowerShell (Windows)

## 📌 O que é PowerShell
- Shell de linha de comando do Windows
- Baseado em objetos (.NET)
- Mais poderoso que CMD

## 📌 Comandos básicos
| Comando | Descrição |
|---------|-----------|
| `Get-ChildItem` | Lista arquivos (ls, dir) |
| `Set-Location` | Muda diretório (cd) |
| `New-Item` | Cria arquivo/pasta |
| `Remove-Item` | Remove (rm, del) |
| `Copy-Item` | Copia (copy, cp) |
| `Move-Item` | Move (move, mv) |
| `Get-Content` | Mostra conteúdo (type, cat) |

## 📌 Aliases
- PowerShell aceita comandos Linux e CMD
- `ls` = `Get-ChildItem`
- `dir` = `Get-ChildItem`
- `cd` = `Set-Location`
- `pwd` = `Get-Location`

## 📌 Variáveis
$nome = "João"
Write-Host "Olá, $nome"

## 📌 Condicionais
if ($a -gt $b) {
  Write-Host "A é maior que B"
} else {
  Write-Host "B é maior que A"
}

## 📌 Loops
for ($i=1; $i -le 5; $i++) {
  Write-Host "Iteração $i"
}

## 📌 Funções
function Saudacao {
  param([string]$nome)
  Write-Host "Olá, $nome!"
}

Saudacao -nome "Amigo"

## 📌 Exemplo: verificar conexões ativas
Get-NetTCPConnection | Where-Object {$_.State -eq "Established"}

## 📌 Exemplo: processos suspeitos (CPU alto)
Get-Process | Where-Object { $_.CPU -gt 50 } | Format-Table Name, CPU, ID

## 📌 Exemplo: verificar chave maliciosa no registro
$chave = "HKCU:\Software\Microsoft\Windows\CurrentVersion\Run\Malware"
if (Test-Path $chave) {
  Write-Host "Chave maliciosa encontrada"
  Remove-Item -Path $chave -Force
} else {
  Write-Host "Nenhuma chave suspeita"
}

## 📌 Exemplo: criptografia simples (AES)
$encryptionKey = [Text.Encoding]::UTF8.GetBytes("MinhaChave123456")
$texto = "SENAI 123"
$bytes = [Text.Encoding]::UTF8.GetBytes($texto)
$aes = [System.Security.Cryptography.Aes]::Create()
$aes.GenerateIV()
$encryptor = $aes.CreateEncryptor()
$encryptedBytes = $encryptor.TransformFinalBlock($bytes, 0, $bytes.Length)
$encryptedText = [Convert]::ToBase64String($aes.IV + $encryptedBytes)
Write-Host "Texto criptografado: $encryptedText"