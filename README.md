# Commands:
`sudo apt install mc yakuake htop curl zsh -y`

# Applications:
## ZSH
### Installation and configuration
* `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
* `apt install fonts-powerline -y`
* `git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k`
* Set `ZSH_THEME="powerlevel10k/powerlevel10k"` in ~/.zshrc.
* `exec zsh`
* Type `p10k configure` if the configuration wizard doesn't start automatically

### for KDE
* `emulate sh -c 'source /etc/profile'`

### Install plugins
* advanced autosuggestion plugin `git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`
* `ls ~/.oh-my-zsh/plugins` and https://github.com/ohmyzsh/ohmyzsh/wiki/Plugins\
in `~/.zshrc` add plugins\
Example `plugins=(git aws terraform docker docker-compose yarn nvm postgres zsh-autosuggestions)`
* `exec zsh`

## enpass https://www.enpass.io/support/kb/general/how-to-install-enpass-on-linux/
* `snap install enpass`
OR
* To install Enpass, add a new repository to /etc/apt/sources.list:
```
sudo -i
echo "deb https://apt.enpass.io/ stable main" > \
  /etc/apt/sources.list.d/enpass.list
```
And import key that is used to sign the release:
```
wget -O - https://apt.enpass.io/keys/enpass-linux.key | tee /etc/apt/trusted.gpg.d/enpass.asc
```
After that, you can install Enpass as any other software package:
```
apt-get update
apt-get install enpass
exit
```
## SDK MAN
* `curl -s "https://get.sdkman.io" | bash`
* `sdk list java`
* `sdk install java 17.0.5-oracle`

## NODE js
```
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash - &&\
sudo apt-get install -y nodejs
```

## YARN
```
npm install --global yarn
```

## Docker
* https://docs.docker.com/engine/install/ubuntu/
* https://docs.docker.com/engine/install/linux-postinstall/

## Terraform
* https://learn.hashicorp.com/tutorials/terraform/install-cli

## AWS
* https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html


# Files
## SSH
* `chmod 700 ~/.ssh `
* `sudo chmod -R 600 ~/.ssh/*`
