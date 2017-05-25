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
