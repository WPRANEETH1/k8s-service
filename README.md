openssl genrsa -out tls.key 2048

openssl req -x509 -new -nodes -key tls.key -sha256 -days 365 -out tls.crt -subj "//CN=example.com/O=My Organization"