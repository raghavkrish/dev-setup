## My Awesome Develeopment environment setup

The Develeopment environment in a machine is very important for a developer and I have tried multiple shells and setups and i'm going to share my best development setup that ive used yet.

Ive been an avid user of fish shell not until very recently, ive moved to zsh. zsh on its own is pretty lameass.. But you can make it extremely cool with a bit of customization and ive been loving it and probably the best setup ive used..


### Install Homebrew
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```


### Install iTerm2
```
brew install --cask iterm2
```

### Install Oh My Zsh
```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Install PowerLevel10K Theme for Oh My Zsh
```
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```


### In ~/.zshrc change the value of ZSH_THEME
```
ZSH_THEME="powerlevel10k/powerlevel10k"
```


### Installing plugins in zsh
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/MichaelAquilina/zsh-auto-notify.git $ZSH_CUSTOM/plugins/auto-notify
git clone https://github.com/MichaelAquilina/zsh-you-should-use.git $ZSH_CUSTOM/plugins/you-should-use
```

### Using the plugins in ~/.zshrc
```
plugins=(zsh-autosuggestions zsh-syntax-highlighting web-search autojump brew auto-notify you-should-use sudo copypath copyfile copybuffer dirhistory history jsontools macos encode64 last-working-dir sublime zsh-interactive-cd)
```




## Setting up iTerm2

* Reopen your iterm2 after this
* Install Meslo Nerd Font - from the prompt
* Set your preferences from the prompt setup as needed
* Voila!

If you are not prompted to install the fonts, you can find them in the fonts folder in this repo. You just have to double click to install the font and set the font in your iterm2 preferences at Profiles>Text>Font

### My additional color theme
* I like to personalize my colors as well and i use coolnight preset which also I have in my assets.
* If you'd like to use it, just download the profile and import it in Profiles>Colors>Color Presets


### Result
![My Terminal](https://github.com/raghavkrish/dev-setup/blob/main/terminal/assets/result/result.png?raw=true)
