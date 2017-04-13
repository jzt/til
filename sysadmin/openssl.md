# openssl

### Decode x509 cert

```
openssl x509 -in cert.pem -text -noout
```

### Show certificate chain

```
openssl s_client -showcerts -connect <IP>:<port>
```
