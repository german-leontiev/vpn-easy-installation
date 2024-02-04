# Setting Up Your Own VPN Server. OpenVPN, WireGuard, and Shadowsocks

## Prerequisites
VPS with Ubuntu 22.04

## Generate keys
```
ssh-keygen
```
### Login to remote VPS
```
ssh -i <PATH_TO_KEY> root@<VPS_IP>
```
## Update system
```
apt update && apt upgrade
```

## Install Wireguard server
```
wget https://git.io/wireguard -O wireguard-install.sh && bash wireguard-install.sh
```

## Install OpenVPN server
```
curl -O https://raw.githubusercontent.com/angristan/openvpn-install/master/openvpn-install.sh
chmod +x openvpn-install.sh
sudo ./openvpn-install.sh
```

## Install Shadowsocks (Outline) server

```
bash -c "$(wget -qO- https://raw.githubusercontent.com/Jigsaw-Code/outline-server/master/src/server_manager/install_scripts/install_server.sh)"
```
