# Expert Sniffle
Simple server activity traching

## Installation

### Pre-requisites
- bash
- ps
- ss
- iotop

### Install
In eslog directory run:
```bash
sudo ./install
```

This copies the eslog script to /usr/local/bin and creates a service file in /etc/systemd/system

### Uninstall
```bash
sudo systemctl disable --now eslog
sudo rm /usr/local/bin/eslog
sudo rm /etc/systemd/system/eslog.service
sudo rm -rf /var/log/eslog
```

## Usage
All usage is done through the web interface.
The default port is 8080 (for the frontend and 3000 for the backend).
```bash
docker-compose up -d
```
