# Ubuntu

## Installation

### After installation
**Update && Upgrade**
```bash
$ sudo apt update
$ sudo apt upgrade
```

**Generate SSH Key && Disable Password Authentication**
```bash
$ ssh-keygen
```

Inside /etc/ssh/sshd_config set PasswordAuthentication directive to no.
```bash
$ sudo vim /etc/ssh/sshd_config
```

And restart the service.
```bash
sudo systemctl restart ssh
```

Create authorized_keys file and add ssh client keys.

**Install zsh && oh-my-zsh**

Install zsh.
```bash
$ sudo apt install zsh
$ zsh --version
```

Make it default shell and restart to use your new default shell.
```bash
$ chsh -s $(which zsh)
```

Install oh-my-zsh via curl.
```bash
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

**Initialize Git global config**

Set name and email.
```bash
$ git config --global user.name 'Your name'
$ git config --global user.email 'youremail@email.com'
```

Set some useful alias.
```bash
$ git config --global alias.co checkout
$ git config --global alias.br branch
$ git config --global alias.cm 'commit -m'
$ git config --global alias.st status
$ git config --global alias.a add
```
