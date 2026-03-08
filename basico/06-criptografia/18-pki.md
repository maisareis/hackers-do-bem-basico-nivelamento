# Aula 18 – Infraestrutura de Chave Pública (PKI)

## 📌 Cartório Digital
- Equivalente ao cartório no mundo físico
- Autoridade Certificadora (CA)

## 📌 Autoridade Certificadora
- Emite certificados digitais
- Certificados são colocados nos sites (cadeado de proteção)
- Certificado emitido por CA = Certificado Assinado

## 📌 Certificado Assinado
- Aspecto de "escadinha" (árvore genealógica)
- Cadeia de confiança

## 📌 Características para ser válido
- Nome correto (Common Name - CN)
- Data e hora válidas
- Não estar revogado
- Ter Autoridade Certificadora válida

## 📌 Certificados Autoassinados
- Possível criar próprio certificado
- Site funciona com HTTPS
- Mas não tem autoridade certificadora atrelada
- Navegador acusa erro (não confiável)

## 📌 Como navegadores sabem a diferença
- Lista interna de CAs confiáveis
- Verificam a cada acesso
- Se certificado não está na lista ou parâmetro incorreto → erro