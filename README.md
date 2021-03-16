# dot_files_revisited


- macOS (reboot and cmd+R)

- Install Xcode from App Store

- Adjust settings

- Install Chrome

### Reinstall Checklist

- Install Alfred

- Install MalwareBytes

- Install Caffeine

- Install Valentina Studio from App Store

- Install Docker Desktop

- Install Xerox B210 and Epson es50

- Install OmniDisk

- Install PGAdmin

-  Install Postman

- Install TeamViewer

- Install VS Code

- Install Sublime Text

- Install Jetbrain toolbox

- Install Android Studio

- Install VLC

- Install Spotify

- Install Signal

- Install Iterm2

- Install zsh

```sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"```

- Create ssh, install github and config

```mkdir -p ~/.ssh && ssh-keygen -t ed25519 -o -a 100 -f ~/.ssh/id_ed25519 -C "EMAIL@HERE.com"```

```cat ~/.ssh/id_ed25519.pub```

add keys to repo

```ssh -T git@github.com``` to check

if does not work: ```ssh-add ~/.ssh/id_ed25519```

```touch ~/.ssh/config``` and write:

```Host *```
  
```AddKeysToAgent yes```
  
```UseKeychain yes```

- Config zsh

```zsh install.sh```
```zsh git_setup.sh```
```touch ~/.aliases```
```nano ~/.zprofile```  --> add : source ~/.aliases
```nano ~/.aliases```  --> Write aliases


- Open Xcode, Install Developer Command Line Tool

- Install GitKraken

- Install brew and first casks


```ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```

```brew update```


```function install_or_upgrade { brew ls | grep $1 > /dev/null; if (($? == 0)); then brew upgrade $1; else brew install $1; fi }```

```install_or_upgrade "git"```

```install_or_upgrade "wget"```


- Install rbenv and install at least ruby 2.6 or 2.7
check also which ruby is used on Mac: https://stackoverflow.com/questions/51126403/you-dont-have-write-permissions-for-the-library-ruby-gems-2-3-0-directory-ma/54873916#54873916

- Install hub

```brew install hub```

- Install node / nvm

https://github.com/nvm-sh/nvm

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash
Nvm install 14
```

- Install Yarn (1 or 2 depending on needs, careful because 2 can be a pain in the...)

- Install Redis

https://redis.io/topics/quickstart

- Install PostGres

https://formulae.brew.sh/formula/postgresql

https://stackoverflow.com/questions/15301826/psql-fatal-role-postgres-does-not-exist

https://www.pgadmin.org/download/

- Install MongoDb Service

https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/

- Install React Native Environment

https://reactnative.dev/docs/environment-setup

https://stackoverflow.com/questions/38495793/run-react-native-application-on-ios-device-directly-from-command-line

- [React DevTool](https://www.npmjs.com/package/react-devtools)

- [Flipper](https://fbflipper.com/)

- [Apollo Developer Tool](https://chrome.google.com/webstore/detail/apollo-client-developer-t/jdkknkkbebbapilgoeccciglkfbmbnfm)

- [Redux DevTool](https://github.com/reduxjs/redux-devtools)

- Gatsby Cli : ```npm install -g gatsby-cli```

- [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli#download-and-install)

- Vercel cli: ```npm i -g vercel@latest```

- [Json viewer](https://chrome.google.com/webstore/detail/json-viewer/gbmdgpbipfallnflgajpaliibnhdgobh)

- [Lastpass](https://www.lastpass.com/)

- [ColorZilla](https://www.colorzilla.com/chrome/)

- [Loom](https://chrome.google.com/webstore/detail/loom-for-chrome/liecbddmkiiihnedobmlmillhodjkdmb)

- [Fullpage screencapture](https://chrome.google.com/webstore/detail/gofullpage-full-page-scre/fdpohaocaechififmbbbbbknoalclacl?hl=en)

- [Wappalyzer](https://chrome.google.com/webstore/detail/wappalyzer/gppongmhjkpfnbhagpmjfkannfbllamg?hl=en)

- [Momentum](https://chrome.google.com/webstore/detail/momentum/laookkfknpbbblfpciffpaejjkokdgca?hl=en)

note: Print the path with `echo -e ${PATH//:/\\n}`
