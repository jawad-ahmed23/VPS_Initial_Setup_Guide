# Setup Guide

## Install NodeJS

### Option 1 - Install NodeJS Directly

```
cd ~
curl -sL https://deb.nodesource.com/setup_20.x -o /tmp/nodesource_setup.sh
```

```
nano /tmp/nodesource_setup.sh
```

```
sudo bash /tmp/nodesource_setup.sh
```

```
sudo apt install nodejs
```

### Option 2 — Installing Node Using the Node Version Manager

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh
```

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```

```
source ~/.bashrc
```

```
nvm list-remote
```

```
nvm install v14.10.0
```

```
nvm install lts/hydrogen
```

```
nvm use v14.10.0
```

## Install Docker

```
# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
```

```
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```
