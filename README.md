# VIMRC and MACOS Settings

## Template guide

[sourabhbajaj mac setup](https://sourabhbajaj.com/mac-setup/)

**Install Xcode**
```
xcode-select --install
```

**Install Homebrew**

**Bash**
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

Add this to your `PATH` environment variable

**for Bash**

``` 
echo 'PATH="/usr/local/bin:$PATH"' >> ~/.bash_profile
```

**for Zsh**

```
echo 'PATH="/usr/local/bin:$PATH"' >> ~/.zshrc
```

## Install iTerm2

```
brew install --cask iterm2
```

**Install OH My ZSH!**

[Oh My ZSH](https://ohmyz.sh/)

```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

**Install Oh My Bash**

[Oh My Bash](https://ohmybash.nntoan.com/)

```
bash -c "$(curl -fsSL https://raw.githubusercontent.com/ohmybash/oh-my-bash/master/tools/install.sh)"
```

##### Setting up Vim

**Install Vim**

```
brew install vim
```

add folder 

```
mkdir .vim && cd .vim
```

add autoload and move the plug.vim at autoload

```
mkdir autoload && mv plug.vim
```

**vimrc Setup and coc**

add the .vimrc at the user's folder

And then at the vim, install the packages in the .vimrc by type :PlugInstall

```
:PlugInstall
```

at Vim install the coc-marketplace

```
:CocInstall coc-marketplace
```

It makes faster to search the previous coc plugins you had before

after installing 
```
:CocList marketplace
```

**My Coc Plugins**

```
coc-json
coc-git
coc-yank
coc-webview
coc-ultisnips
coc-tabnine
coc-spell-checker
coc-snippets
coc-scssmodules
coc-neosnippet
coc-marketplace
coc-just-complete
coc-html-css-support
coc-html
coc-highlight
coc-fzf-preview
coc-emmet
coc-dash-complete
coc-cssmodules
coc-tsserver
coc-yaml
coc-browser
coc-sh
coc-yaml
coc-jsref
coc-htmlhint
coc-css
```

**Coc auto plugin install**

be sure that this is available in the vimrc

```
"Vim COC Plugins
let g:coc_global_extensions = ['coc-json', 'coc-git', 'coc-yank', 'coc-webview', 'coc-ultisnips', 'coc-tabnine', 'coc-spell-checker', 'coc-snippets', 'coc-scssmodules', 'coc-neosnippet', 'coc-marketplace', 'coc-just-complete', 'coc-html-css-support', 'coc-html', 'coc-highlight', 'coc-fzf-preview', 'coc-emmet', 'coc-dash-complete', 'coc-cssmodules', 'coc-tsserver', 'coc-yaml', 'coc-browser', 'coc-sh', 'coc-yaml', 'coc-jsref', 'coc-htmlhint', 'coc-css']
```
It will automatically install the plugins which aren't available

## Install FZF and more

[Chris@Machine FZF](https://www.chrisatmachine.com/Neovim/08-fzf/)

[FZF will change your workflow completely](https://www.youtube.com/watch?v=on1AzaZzQ7k&t=287s)
