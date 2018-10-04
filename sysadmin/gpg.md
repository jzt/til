# gpg

### Symmetric encryption
```
gpg --output encrypted.data --symmetric --cipher-algo AES256 un_encrypted.data
gpg --output un_encrypted.data --decrypt encrypted.data
```
