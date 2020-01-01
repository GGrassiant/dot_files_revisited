# dot_files_revisited

- ***install iTerm***

- ***Install zsh***

sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

- ***Link Github***

mkdir -p ~/.ssh && ssh-keygen -t ed25519 -o -a 100 -f ~/.ssh/id_ed25519 -C "TYPE_YOUR_EMAIL@HERE.com"

cat ~/.ssh/id_ed25519.pub

ssh -T git@github.com or ssh-add ~/.ssh/id_ed25519

- ***dotfiles and config***

export GITHUB_USERNAME=replace_this_with_your_github_username

mkdir -p ~/code/$GITHUB_USERNAME && cd $_ && git clone git@github.com:$GITHUB_USERNAME/dot_files_revisited.git

cd ~/code/$GITHUB_USERNAME/dotfiles

zsh install.sh

cd ~/code/$GITHUB_USERNAME/dotfiles

zsh git_setup.sh

sw_vers

touch ~/.ssh/config and write

Host *
  
  AddKeysToAgent yes
  
  UseKeychain yes

- ***For keyboard*** 

Alfred with double tap on CMD

- ***IDE profile*** 

from jetBrain online
