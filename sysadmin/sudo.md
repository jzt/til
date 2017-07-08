# sudo

### Add new sudo user

```
visudo

<username>  ALL=(ALL:ALL) ALL
```


### Passwordless sudo

```
visudo

<username>  ALL=(ALL:ALL) NOPASSWD:ALL
```
