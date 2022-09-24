# Ubuntu 22.04

Install Ubuntu 22.04:

https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10


# Update

```bash
sudo apt update
sudo apt upgrade -y
```


# Enable Docker Desktop Integration

Docker Desktop
Settings 
-> Resources
-> WSL Integration 
-> Enable Integration with additional distros:
Ubuntu-22.04


https://docs.docker.com/engine/install/linux-postinstall/

```bash
sudo usermod -aG docker $USER
newgrp docker 
```

# Install GO

```bash
sudo apt install golang-go -y
```


