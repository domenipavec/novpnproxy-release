# novpnproxy-release

This repository contains releases of novpnproxy

## Install

### Debian/Ubuntu

1. Add repository key:
```sh
wget -qO - https://domenipavec.github.io/novpnproxy-release/deb/conf/novpnproxy.gpg.key | sudo apt-key add -
```

2. Add repository:
```sh
echo "deb https://domenipavec.github.io/novpnproxy-release/deb stable main" | sudo tee /etc/apt/sources.list.d/novpnproxy.list
```

3. Update and install
```sh
sudo apt update
sudo apt install novpnproxy-client
```

## Configure as a service

```sh
sudo novpnproxy-client --client_id <CLIENT_ID> --client_token <TOKEN> install
sudo novpnproxy-client start
```
