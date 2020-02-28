# dot_files_revisited

- ***install iTerm***

- ***Install zsh***

sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

- ***Link Github***

mkdir -p ~/.ssh && ssh-keygen -t ed25519 -o -a 100 -f ~/.ssh/id_ed25519 -C "TYPE_YOUR_EMAIL@HERE.com"

cat ~/.ssh/id_ed25519.pub

pbcopy < ~/.ssh/id_rsa.pub

akouter les clef dans le repo or ssh-add ~/.ssh/id_ed25519

ssh -T git@github.com to check

- ***dotfiles and config***

touch ~/.ssh/config and write:

Host *
  
  AddKeysToAgent yes
  
  UseKeychain yes

- ***For keyboard*** 

Alfred with double tap on CMD

- ***IDE profile*** 

from jetBrain online

git config --global core.editor "nano"

***more aliases***
touch ~/.aliases

nano ~/.zprofile  --> Ajouter : source ~/.aliases

nano ~/.aliases  --> Mettre tes alias

https://github.com/rbenv/rbenv

install:

- node
- nvm
- npm
- homebrew
- yarn
- react native deps
