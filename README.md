# dot_files_revisited

- ***make sure xcode is installed***

```xcode-select --install``` -- also check app store

- ***Install Homebrew and git***

```ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```

```brew update```


```function install_or_upgrade { brew ls | grep $1 > /dev/null; if (($? == 0)); then brew upgrade $1; else brew install $1; fi }```

```install_or_upgrade "git"```

```install_or_upgrade "wget"```

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

```https://github.com/rbenv/rbenv```

install ruby 2.6

```brew install hub```

- ***config***

```zsh install.sh```
```zsh git_setup.sh```


```touch ~/.ssh/config``` and write:


```Host *```
  
```AddKeysToAgent yes```
  
```UseKeychain yes```

```git config --global core.editor "webstorm"``` or ```git config --global core.editor "code --wait"```

- ***Install Alfred*** 

https://www.alfredapp.com/

- ***Install IDE*** 

https://www.jetbrains.com/toolbox-app/


- ***Install GITKraken*** 

https://www.gitkraken.com/download/mac


- ***Install Postman*** 

https://www.postman.com/


- ***more aliases***

```touch ~/.aliases```

```nano ~/.zprofile```  --> add : source ~/.aliases

```nano ~/.aliases```  --> Write aliases

- ***Install node and npm/nvm***

https://nodejs.org/en/
  
https://github.com/nvm-sh/nvm

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash
Nvm install 14
```

https://classic.yarnpkg.com/en/docs/install/#mac-stable

- ***Install Docker and Docker Desktop***

https://docs.docker.com/get-docker/

- ***Install Redis***

https://redis.io/topics/quickstart

- ***Install PostgreSQL & PGAdmin***

https://formulae.brew.sh/formula/postgresql

https://stackoverflow.com/questions/15301826/psql-fatal-role-postgres-does-not-exist

https://www.pgadmin.org/download/

- ***Install MongoDb***

https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/

- ***Install React Native Deps***

https://reactnative.dev/docs/environment-setup

- ***Others***

install:
- [React DevTool](https://www.npmjs.com/package/react-devtools)
- [Flipper](https://fbflipper.com/)
- [Apollo Developer Tool](https://chrome.google.com/webstore/detail/apollo-client-developer-t/jdkknkkbebbapilgoeccciglkfbmbnfm)
- [Redux DevTool](https://github.com/reduxjs/redux-devtools)
- Gatsby Cli : ```npm install -g gatsby-cli```
- [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli#download-and-install)
- Vercel cli: ```npm i -g vercel@latest```
- Netlify cli: ```https://docs.netlify.com/cli/get-started/#installation```
- [Json viewer](https://chrome.google.com/webstore/detail/json-viewer/gbmdgpbipfallnflgajpaliibnhdgobh)
- [Lastpass](https://www.lastpass.com/)
- [ColorZilla](https://www.colorzilla.com/chrome/)
- [Loom](https://chrome.google.com/webstore/detail/loom-for-chrome/liecbddmkiiihnedobmlmillhodjkdmb)
- [Fullpage screencapture](https://chrome.google.com/webstore/detail/gofullpage-full-page-scre/fdpohaocaechififmbbbbbknoalclacl?hl=en)
- [Wappalyzer](https://chrome.google.com/webstore/detail/wappalyzer/gppongmhjkpfnbhagpmjfkannfbllamg?hl=en)
- [Momentum](https://chrome.google.com/webstore/detail/momentum/laookkfknpbbblfpciffpaejjkokdgca?hl=en)

note: Print the path with `echo -e ${PATH//:/\\n}`
