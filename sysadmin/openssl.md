# openssl

### Decode x509 cert

```
openssl x509 -in cert.pem -text -noout
```

### Show certificate chain

```
openssl s_client -showcerts -connect <IP>:<port>
```

### Get fingerprint of remote server

```
openssl s_client -connect <IP>:<port> < /dev/null 2>/dev/null | openssl x509 -fingerprint -noout -in /dev/stdin
```

### Get fingerprint of certificate

```
openssl x509 -in server.crt -noout -sha256 -fingerprint
```

### PEM to CRT
```
openssl x509 -outform der -in starkenterprises.io.cert.pem -out starkenterprises.io.crt
```

### PEM to PKCS8
```
openssl pkcs8 -topk8 -inform PEM -outform PEM -nocrypt -in starkenterprises.io.key.pem -out starkenterprises.io.key.pkcs8
```
