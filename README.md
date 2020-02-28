# dot_files_revisited

- ***make sure xcode is installed***
```xcode-select --install```

- ***Install Homebrew***
```ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```

```brew update```

```function install_or_upgrade { brew ls | grep $1 > /dev/null; if (($? == 0)); then brew upgrade $1; else brew install $1; fi }```
```install_or_upgrade "git"```
```install_or_upgrade "wget"```
```install_or_upgrade "imagemagick"```
```install_or_upgrade "jq"```
```install_or_upgrade "openssl"```

- ***install iTerm***
https://iterm2.com/

- ***Install zsh***

```sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"```

- ***Link Github***

```mkdir -p ~/.ssh && ssh-keygen -t ed25519 -o -a 100 -f ~/.ssh/id_ed25519 -C "EMAIL@HERE.com"```

```cat ~/.ssh/id_ed25519.pub```

add keys to repo

```ssh -T git@github.com``` to check

if does not work: ```ssh-add ~/.ssh/id_ed25519```

- ***config***
```zsh install.sh```
```zsh git_setup.sh```


```touch ~/.ssh/config``` and write:


```Host *```
  
```AddKeysToAgent yes```
  
```UseKeychain yes```

```git config --global core.editor "nano"```

- ***Install Alfred*** 

https://www.alfredapp.com/

- ***Install IDE*** 

https://www.jetbrains.com/toolbox-app/

***more aliases***
touch ~/.aliases

nano ~/.zprofile  --> add : source ~/.aliases

nano ~/.aliases  --> Write aliases

***Others***
install:
- node
- nvm
- npm
- yarn
- react native deps
