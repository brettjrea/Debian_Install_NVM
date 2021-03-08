# Debian_Install_NVM

Install NVM on Debian with Curl and Bash script.

---

## Commands:
```
sudo apt install curl &&
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash &&
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" 
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion" &&
```

*If you can't copy and paste the above command, close and reopen the terminal to start using NVM and continue.*

```
nvm install LTS
```

---

*You might now want to [install Strapi.io](https://github.com/brettjrea/Debian_Strapi_Backend_API) backend*
