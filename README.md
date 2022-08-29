# shichihara dotfiles

## Quick Start

執行 `script/bootstrap`
```
sh ./script/bootstrap
```
`bootstrap` 腳本會自動完成以下工作
1. 檢查並安裝 [Homebrew](http://brew.sh/)。
2. 安裝 Homebrew packages (binaries, apps)
3. 檢查並安裝 [Oh My Zsh](http://ohmyz.sh/)。
4. 檢查並匯入 dotfiles
5. 安裝vscode常用套件及匯入`setting.json`

### Homebrew packages

執行 `bin/dot` 的時候，腳本會根據 `Brewfile` 使用 Homebrew 和 Homebrew Cask 來安裝，目前安裝的packages:

需要增減binaray package，可以用
`
brew search XXX
`
或到 [Homebrew Formulae](https://formulae.brew.sh/) 搜尋package是否存在
```
brew 'bash'
...
```

需要增減app package，可以用 `brew cask search XXX` 或到 [Homebrew Formulae](https://formulae.brew.sh/) 搜尋package是否存在
```
cask 'google-chrome'
...
```

#### Binaries

| name | 說明 |
| --- | --- |
| [git-cola](https://git-cola.github.io/) | git管理套件 |
| [mongodb](https://www.mongodb.com/) | 資料庫套件 |
| [nvm](https://github.com/nvm-sh/nvm) | Node版本控制 |
| [mySQL](http://ftp.ntu.edu.tw/MySQL/Downloads/MySQL-5.7/) | 資料庫套件 |
| zsh | |

#### Apps

| name | 說明 |
| --- | --- |
| [Firefox](https://www.mozilla.org/zh-TW/firefox/new/) | |
| [GitHub Desktop](https://desktop.github.com/) | |
| [Google Chrome](https://www.google.com/intl/zh-TW/chrome/) | |
| [iterm2](https://iterm2.com/) | |
| [MySQL Workbench](https://dev.mysql.com/downloads/workbench/) | 資料庫管理 |
| [Postman](https://www.postman.com/) | |
| [Sequel Pro](https://sequelpro.com/) | 資料庫管理 |
| [slack](https://slack.com/intl/zh-tw/) | 通訊軟體 |
| [spotify](https://open.spotify.com/) | |
| [Visual Studio Code](https://code.visualstudio.com/) | |
| [zeplin](https://zeplin.io/) | 設計協作工具 |

### iterm2 setting

參考 `iterm` 內檔案

### 額外設定指令

設定zsh為預設
```
chsh -s $(which zsh)
```

nvm設定預設開啟node版本
```
nvm alias default {version}
```

## References
 - [如何優雅地在 Mac 上使用 dotfiles?](https://segmentfault.com/a/1190000002713879) [[github](https://github.com/amowu/dotfiles)]