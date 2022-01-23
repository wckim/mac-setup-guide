## 기본 개발 환경

* 개발 환경
```bash
$ brew install nvm
$ brew install pyenv
$ brew install pyenv-virtualenv
$ brew install jenv
```

* 폰트 설치
```bash
$ brew tap homebrew/cask
$ brew tap homebrew/cask-fonts
$ brew install font-d2coding
```


## iTerm2 설정

* 설치
```bash
brew install iterm2
```

* 설정
- 한글 깨짐: Profile -> Text -> Unicode 항목에서 "Unicode normalization form" 옵션을 기존 "None"에서 "NFC"로 변경



## oh-my-zsh

* 설치
```bash
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

* 설정 (테마/플러그인 설치)
```bash
$ git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
$ git clone --depth=1 https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/zsh-autosuggestions 
$ git clone --depth=1 https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
$ git clone --depth=1 https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions

```


## Visual Studio Code

* 설치
```bash
$ brew install visual-studio-code
```

* 설정 (플러그인 설치)
- eslit
- prettier


## Sublime Text

* 설치
```bash
$ brew install subline-text
```

## Dropbox

* 설치
```bash
$ brew install dropbox
```


## GNUPG

* 설치
```bash
$ brew install gnupg
```

* 설정

- 저장한 키 복원 
```bash
$ gpg —-import /path/to/secret-key-backup.asc  # 저장한 키 파일 

$ gpg --edit-key 5A06ATD1F983B0A0 # Replace "name" with yours

$ gpg> trust # Choose "ultimate" or other trust level
$ gpg> save # Save the changes
```

- git config 설정
```bash
$ git config --global user.signingkey 5A06ATD1F983B0A0
$ git config --global gpg.program /opt/homebrew/bin/gpg
$ git config --global commit.gpgsign true
$ git config --global alias.undo 'reset --soft HEAD~1'
$ git config --global alias.lg 'log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit'
```


## Java & Jenv

* 설치
```bash
$ brew tap mdogan/zulu
$ brew install zulu-jdk8
$ brew install zulu-jdk11
$ brew install zulu-jdk17
```

* 설정
```bash
$ jenv add /Library/Java/JavaVirtualMachines/zulu-8.jdk/Contents/Home
$ jenv add /Library/Java/JavaVirtualMachines/zulu-11.jdk/Contents/Home
$ jenv add /Library/Java/JavaVirtualMachines/zulu-17.jdk/Contents/Home
```
