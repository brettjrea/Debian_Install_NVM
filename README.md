# Debian_Install_NVM

Install NVM and NPM LTS on Debian/Ubuntu with Curl and Bash script.

---
##### Updated to v0.39.3 02/2023

#### This new one fetches a script from this repo.

```
sudo apt upgrade -y && sudo apt update -y && sudo apt autoremove -y &&
sudo apt install wget &&
sudo apt-get install --reinstall ca-certificates -y &&
wget https://raw.githubusercontent.com/brettjrea/Debian_Install_NVM/main/install-nvm.sh &&
chmod +x install-nvm.sh &&
./install-nvm.sh &&
sudo apt autoremove -y &&
sudo apt clean -y
```
---

### This is the original commands only:

```
sudo apt upgrade -y && sudo apt update -y && sudo apt autoremove -y
sudo apt install curl -y
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" 
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"
nvm install --lts
```

---
## Script breakdown:

### Always be updating:

```

sudo apt upgrade -y && sudo apt update -y && sudo apt autoremove -y

```

### Install required programs:

```
sudo apt install curl -y
```

### Download NVM installer script with Curl:

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```

### Add environmental variables:

```
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" 
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"
```

*You may need to close and reopen the terminal to start using NVM and run the following command to install LTS.*

### Use NVM to install NPM LTS:

```
nvm install --lts
```

---

*You might now want to [install Strapi.io](https://github.com/brettjrea/Debian_Strapi_Backend_API) backend*
