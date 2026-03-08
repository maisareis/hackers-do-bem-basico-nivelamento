# Aula 2 – Web: HTTP e HTTPS

## 📌 Como funciona
1. Navegador interpreta URL (protocolo + servidor + arquivo)
2. Consulta DNS para converter nome em IP
3. Envia requisição HTTP/HTTPS
4. Servidor responde com código HTML
5. Navegador decifra e formata página

## 📌 Métodos HTTP
- **GET** → solicitar dados
- **POST** → enviar dados (formulários)
- **PUT** → carregar/atualizar recurso
- **DELETE** → remover recurso
- **PATCH** → modificar parte de recurso

## 📌 HTTP
- Protocolo de transferência de hipertexto
- Porta 80
- Não seguro (dados em texto claro)
- Mensagens podem ser interceptadas

## 📌 HTTPS
- HTTP com SSL/TLS
- Porta 443
- Criptografado
- Autentica o servidor
- Protege contra interceptação

## 📌 Importante
- HTTPS não garante que site é confiável
- Apenas garante comunicação criptografada
- Certificado digital atesta identidade