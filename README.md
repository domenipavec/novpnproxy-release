# novpnproxy-release

This repository contains releases of novpnproxy

## Adding apt repository

1. Add repository key:
```sh
wget -qO - https://domenipavec.github.io/novpnproxy-release/deb/conf/novpnproxy.gpg.key | sudo apt-key add -
```

1. Add repository:
```sh
echo "deb https://domenipavec.github.io/novpnproxy-release/deb stable main" | sudo tee /etc/apt/sources.list.d/novpnproxy.list
```

1. Update and install
```sh
sudo apt update
sudo apt install novpnproxy-client
```
