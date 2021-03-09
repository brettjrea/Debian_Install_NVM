# Debian_Install_NVM

Install NVM and NPM LTS on Debian with Curl and Bash script.

---

## Quickscript:

```
sudo apt upgrade -y && sudo apt update -y && sudo apt autoremove -y


## Always be updating:

```
sudo apt upgrade -y && sudo apt update -y && sudo apt autoremove -y

sudo apt install curl

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" 
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"

nvm install --lts
```

---

## Install required programs:

```
sudo apt install curl
```

---

## Commands:
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```

```
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" 
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"
```

*You may need to close and reopen the terminal to start using NVM and run the following command to install LTS.*

```
nvm install --lts
```

---

*You might now want to [install Strapi.io](https://github.com/brettjrea/Debian_Strapi_Backend_API) backend*
