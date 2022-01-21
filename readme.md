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
```


## Visual Studio Code

* 설치
```bash
brew install visual-studio-code
```

* 설정 (플러그인 설치)
- eslit
- prettier


## Sublime Text

* 설치
```bash
brew install subline-text
```
