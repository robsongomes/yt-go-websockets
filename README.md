# Geração do par de chaves

```bash
# gera a chave privada
openssl genrsa -out server.key 2048

# gera a chave pública a partir da chave privada
openssl req -new -x509 -sha256 -key server.key -out server.crt -days 365

```