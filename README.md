# LapTop_Update_Log



# MacBook Pro 16 inch

- 2024/08/03 → `~/.zshrc` file  `export LANG=en_US.UTF-8` 주석 해제
- 2024/08/13 → **Amphentamine App On/Off 단축키 설정** (`shift` + `command` + ‘`+`’) / (`shift` + `command` + ‘`-`’) → Macbook Air 와 동일하게 설정함
- 2024/08/13 → Intelli J (keymap edit) remove : `^` + `→` , `←` → Macbook Air 와 동일하게 설정함
- 2024/08/17 → VS Code : shell 명령어로 `>shell` 입력해서 termianl 에서 code 로 vsCode 여는거 설치 **(MacBook Pro first)**
- 2024/08/17 → mac Sublime Text code → Sublime Text Update **(Macbook Pro second)**
    
    ```bash
    sudo ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
    
    ```
    

- 2024/08/17 → `brew install tmux`  **(Macbook Pro first)**

- 2024/08/18 → `brew bundle dump` 명렁어로 brew installed file 생성 **(Macbook Pro second)**
- 2024/08/18 → `brew install --cask mongodb-compass`  **(Macbook Pro second)**
- 2024/08/18 → Memory Diag  설치 <App Store>  **(Macbook Pro second)** → Open at Login & Dark Theme & Colored Memorial Details
- 2024/08/18 → lazyvim colorscheme change **(Macbook Pro second)**
    
    make `~/.config/nvim/lua/plugins/colorscheme.lua` and 
    
    ```lua
    return {
      {
        "LazyVim/LazyVim",
        opts = {
          colorscheme = "tokyonight-night",
        },
      },
    }
    ```
    
- 2024/08/18 → Chorme Vimium 설치함 **(Macbook Pro second)**
- 2024/08/18 → R & R Studio 삭제

- 2024/08/18 → Chrome 확장 프로그램 : Vimium → `https?://www.youtube.com/*` exclude **(Macbook Pro first)** → **아마도 Macbook Air 저절로 동기화 될거 같긴한데..**

- 2024/08/20 → `brew install --cask warp` : warp 터미널 설치 **(Macbook Pro second)**
- 2024/08/20 → `~/.config/nvim/lua/config/options.lua` file add `vim.opt.relativenubmer = false`  → 절대 줄 번호로 바꿈 **(Macbook Pro second)**
- 2024/08/20 → `brew install zsh-syntax-highlighting`   **(Macbook Pro first)**
- 2024/08/20 → `brew install --cask obsidian` : obsidian 설치 **(Macbook Pro second)**
- 2024/08/20 → `git clone [https://github.com/github/copilot.vim](https://github.com/github/copilot.vim) \~/.config/nvim/pack/github/start/copilot.vim`  : Lazyvim Copilot Install **(Macbook Pro second)**

- 2024/08/21 → 시스템 설정/키보드/단추키 설정 : Dock으로 초점 이동 → `command + shift + ,` **(Macbook Pro second)**
- 2024/08/21 → Memory Diag APP Colored Memory Details : 무색으로 변경 **(Macbook Pro second)**

- 2024/08/22 → Obsidian 커뮤니티 플러그인 : execute code 설치 **(Macbook Pro second)**
- 2024/08/22 → `brew install ripgrep` **(Macbook Pro second)**
- 2024/08/22 → `npm install -g neovim` **(Macbook Pro second)**
- 2024/08/22 → `~/.config/nvim/lua/config/options.lua` → add `vim.opt.winbar = “%=%m %f”` **(Macbook Pro second)**
- 2024/08/22 → nvim : LazyExtras : `coding.copilot plugins` → <x>key to disable change **(Macbook Pro second)**
- 2024/08/22 → LazyVim plugins <ui.mini-animate> change to enable plugins **(Macbook Pro first)**

- 2024/08/23 → PyCharm update → (keymap edit) remove : `^` + `→` , `←` & Copilot disable and update **(Macbook Pro second)**
- 2024/08/23 → LazyVim TabOut Plugins install → `~/.config/nvim/lua/plugins/tabout.lua`  file add & add Code **(Macbook Pro second)**
    
    [tabout.lua](LapTop%20UpDate%20Log/tabout.lua)
    
- 2024/08/23 → `brew install lua` : lua installed **(Macbook Pro second)**
- 2024/08/23 → LazyVim ScrollBar Plugins install `~/.config/nvim/lua/plugins/scrollbar.lua` fie add & add Code→ **(Macbook Pro second)**
    
    [scrollbar.lua](LapTop%20UpDate%20Log/scrollbar.lua)
    

- 2024/08/23 → VSCode : <vscode-pdf> plugins installed **(Macbook Pro first)**

- 2024/08/24 → LazyVim Extras : lang plugins install **(Macbook Pro second)**
- 2024/08/24 → Intellij IDEA : <IdeaVim> Plugin install **(Macbook Pro first)**
- 2024/08/24 → Discord Update **(Macbook Pro second)**

- 2024/08/24 → alias command change → `ls` to `lsd` `/Users/parksangmin/.oh-my-zsh/lib/directories.zsh` file edit **(Macbook Pro first)**
    
    ```bash
    
        ~/.oh-my-zsh/lib    master !2 ?2 ─────────────────────────────────────────────── 3m 38s   02:11:32  
    ❯ cat directories.zsh
    # Changing/making/removing directory
    setopt auto_cd
    setopt auto_pushd
    setopt pushd_ignore_dups
    setopt pushdminus
    
    alias -g ...='../..'
    alias -g ....='../../..'
    alias -g .....='../../../..'
    alias -g ......='../../../../..'
    
    alias -- -='cd -'
    alias 1='cd -1'
    alias 2='cd -2'
    alias 3='cd -3'
    alias 4='cd -4'
    alias 5='cd -5'
    alias 6='cd -6'
    alias 7='cd -7'
    alias 8='cd -8'
    alias 9='cd -9'
    
    alias md='mkdir -p'
    alias rd=rmdir
    
    function d () {
      if [[ -n $1 ]]; then
        dirs "$@"
      else
        dirs -v | head -n 10
      fi
    }
    compdef _dirs d
    
    # List directory contents
    alias lsa='lsd -lah'  -> 수정한 부분 2024/08/25
    alias l='lsd -lah' -> 수정한 부분 2024/08/25
    alias ll='lsd -lh'  -> 수정한 부분 2024/08/25
    alias la='lsd -lAh'  -> 수정한 부분 2024/08/25
    ```
    
- 2024/08/25 → `brew install fd`  **(Macbook Pro first)**

- 2024/08/25 → 시스템 설정/제어 센터/배터리/퍼센트 잔량 보기 설정 **(Macbook Pro first)**
- 2024/08/25 → `brew install --cask keka` **(Macbook Pro second)**

- 2024/08/27 → ChatGPT_Desktop_public_latest.dmg install & Chrome App ChatGPT remove **(Macbook Pro second)**
    
    [ChatGPT on desktop](https://openai.com/chatgpt/mac/)
    
- 2024/08/27 → Lazyvim : <vim-visual-multi> plugin install → lua/plugin/visual-multi.lua file add & code insert **(Macbook Pro second)**
- 2024/08/27 → `brew install htop` **(Macbook Pro second)**
    
    [[macOS] htop을 이용하여 mac을 관리하기](https://sukvvon.tistory.com/37)
    

- 2024/08/28 → `brew install nyancat`  **(Macbook Pro second)**
- 2024/08/28 → `brew install asciiquarium`  **(Macbook Pro first)**
- 2024/08/28 → `brew install docker`  **(Macbook Pro second)**
- 2024/08/28 → `brew install font-jetbrains-mono` **(Macbook Pro first)**
- 2024/08/28 → `brew install tig` **(Macbook Pro first)**

- 2024/08/28 → `brew install zsh` **(Macbook Pro first)**
- 2024/08/28 → `brew install zsh-completions` **(Macbook Pro second)**
- 2024/08/28 → `brew install fzf` **(Macbook Pro first)**

- 2024/08/29 → `brew install bat` && `~/.zshrc` file edit **(Macbook Pro second)**
    
    add `alias cat=’bat --paging never’`
    
- 2024/08/29 → **iterm2** Settings : Cursor Colors → **Cursor Text (HSB with Hue Slider) Black** & **Smart Box coursor color** → checked **(Macbook Pro second)**
    - **커서 배경색**: #F0F0F0 (밝은 회색)
    - **커서 텍스트 색상**: #000000 (검정색)

- 2024/08/30 → `brew install pstree` **(Macbook Pro second)**

- 2024/09/04 → `brew install lazydocker` **(Macbook Pro second)**
- 2024/09/04 → `~/.zshrc` file edit `<lazydocker>` **(Macbook Pro second)**
    
    add `alias ldk=’lazydocker’`
    

- 2024/09/04 → `brew install docker-compose` **(Macbook Pro second)**
- 2024/09/04 → `brew install wget` **(Macbook Pro second)**
- 2024/09/04 → `brew install --cask figma` **(Macbook Pro second)**
- 2024/09/04 → `~/.zshrc` file edit : plugins add `web-search` **(Macbook Pro second)**
    
    ```bash
    plugins=(git zsh-syntax-highlighting zsh-autosuggestions autojump web-search)
    ```
    

- 2024/09/05 → `brew install gitui` **(Macbook Pro second)**
- 2024/09/05 → `~/.zshrc` file edit `<gitui>` **(Macbook Pro second)**
    
    add `alias gu=’gitui’`
    
- 2024/09/05 → `brew install lazygit` **(Macbook Pro second)**
- 2024/09/05 → `~/.zshrc` file edit `<lazygit>`**(Macbook Pro second)**
    
    add `alias lg=’lazygit’`
    

- 2024/09/08 → `brew install tpm` **(Macbook Pro second)**
- 2024/09/08 → `touch ~/.tmux.conf` **(Macbook Pro second)**
- 2024/09/08 → Clone TPM **(Macbook Pro second)**
    
    ```bash
    git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
    ```
    

- 2024/09/09 → `pip install powerline-status` **(Macbook Pro second)**
- 2024/09/09 → `pip install psutil` **(Macbook Pro second)**
- 2024/09/09 → `pip install dbus-python` **(Macbook Pro second)**
- 2024/09/09 → `powerline-config tmux setup` **(Macbook Pro second)**

- `.tmux.conf` file **(Macbook Air / Pro)**
    
    ```bash
    if-shell 'test -z "$POWERLINE_CONFIG_COMMAND"' 'set-environment -g POWERLINE_CONFIG_COMMAND powerline-config'
    
    # Don't version-check for this core functionality -- anything too old to
    # support these options likely won't work well with powerline
    
    set-option -g focus-events on
    
    set -g status on
    set -g status-interval 2
    set -g status-left-length 70
    #set -g status-left "#(powerline tmux left)"
    #set -g status-left '#[fg=colour235,bg=colour252,bold] #S #[fg=colour252,bg=colour238,nobold]#[fg=colour245,bg=colour238,bold] #(whoami) #[fg=colour238,bg=colour234,nobold]'
    
    set -g status-right-length 150
    set -g status-right "#(powerline tmux right)"
    set -sg escape-time 0
    #set -g status-right '#[fg=colour59]#[fg=colour255,bg=colour59] #[fg=colour254,bold]#[fg=colour16,bg=colour254,bold] #h '
    
    set -g window-status-separator '#[fg=colour244,bg=colour234]'
    set -g window-status-format "#[fg=colour244,bg=colour234] #I #[fg=colour240] #[default,bg=colour234]#W "
    set -g window-status-current-format "#[fg=colour234,bg=colour31]#[fg=colour117,bg=colour31] #I  #[fg=colour231,bold]#W #[fg=colour31,bg=colour234,nobold]"
    
    # Key bind
    bind-key -n C-S-Left previous-window
    bind-key -n C-S-Right next-window
    
    # bind-key -n C-M-k select-pane -U
    # bind-key -n C-M-j select-pane -D
    # bind-key -n C-M-h select-pane -L
    # bind-key -n C-M-l select-pane -R 
    
    #Set Mouse
    set -g mouse on
    
    set -g history-limit 100000
    
    setw -g mode-keys vi
    
    # Moving Windows
    bind-key -r Left swap-window -t -1\; select-window -t -1
    bind-key -r Right swap-window -t +1\; select-window -t +1
    
    bind -r k select-pane -U
    bind -r j select-pane -D
    bind -r h select-pane -L
    bind -r l select-pane -R 
    
    # load powerline
    if-shell 'env "$POWERLINE_CONFIG_COMMAND" tmux setup' '' 'run-shell "powerline-config tmux setup"'
    
    ```
    
- 2024/09/09 → `unset TMUX` **(Macbook Pro second)**
- 2024/09/09 → `scutil --set HostName Park_Sang_Min` **(Macbook Pro second)**
- 2024/09/09 → `~/.zshrc` file edit `<tmux>`**(Macbook Pro second)**
    
    add `alias t=’tmux’`
    

- 2024/09/10 → vscode HTML CSS Support install
- 2024/09/10 → `brew install --cask cursor` **(Macbook Pro second)**

- 2024/09/11 → `brew install nvtop` **<GPU 사용량 모니터링> (Macbook Pro second)**
- 2024/09/11 → `sudo npm install -g vtop`  **(Macbook Pro second)**
- 2024/09/11 → `brew install git-octopus` **(Macbook Pro second)**
- 2024/09/11 → `brew install git-open` **(Macbook Pro second)**
- 2024/09/11 → `brew install coreutils` **(Macbook Pro second)**
- 2024/09/11 → `brew install gnu-sed` **(Macbook Pro second)**
- 2024/09/11 → `brew install osx-cpu-temp` **(Macbook Pro second)**
- 2024/09/11 → install `bashtop`
    
    ```bash
    git clone [https://github.com/aristocratos/bashtop.git](https://github.com/aristocratos/bashtop.git)
    cd bashtop
    sudo make install
    ```
    
- 2024/09/11 → `brew install bash` **(Macbook Pro second)**
- 2024/09/11 → `brew install python3` **(Macbook Pro second)**
- 2024/09/11 → `brew install pipx` **(Macbook Pro second)**
- 2024/09/11 → bash -version upgade
    
    ```bash
    2019  curl -O [https://ftp.gnu.org/gnu/bash/bash-5.0.tar.gz](https://ftp.gnu.org/gnu/bash/bash-5.0.tar.gz)
    2022  tar -xvf bash-5.0.tar.gz
    2025  cd bash-5.0
    2028  ./configure
    2029  make
    2030  make install
    ```
    

- 2024/09/11 → `python3 -m pip config set global.break.system-packages ture`
- 2024/09/11 → `brew install ack` **(Macbook Pro second)**
- 2024/09/12 → `~/.tmux.conf` file edit **(Macbook Pro second)**
    
    ```bash
    set -g escape-time 0 
    
    bind-key -n C-S-Left previous-window
    bind-key -n C-S-Right next-window
    ```
    

- 2024/09/13 → `~/.tmux.conf` file edit **(Macbook Pro first)**
    
    ```bash
    bind-key -n C-S-Left previous-window
    bind-key -n C-S-Right next-window
    
    bind -r k select-pane -U
    bind -r j select-pane -D
    bind -r h select-pane -L
    bind -r l select-pane -R 
    ```
    
- 2024/09/13 → neovim Mason `html-lsp` install **(Macbook Pro first)**

- 2024/11/02 → 시스템 설정/키보드/키보드 단축키/입력 소스/ `이전 입력 소스 선택 해제`
- 2024/11/02 → `brew install npm`
- 2024/11/02 → **MacBook Air Software Update**
- 2024/09/21 → Dock **Slack, Stats** 제거

![Before](LapTop%20UpDate%20Log/%25E1%2584%2589%25E1%2585%25B3%25E1%2584%258F%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25B5%25E1%2586%25AB%25E1%2584%2589%25E1%2585%25A3%25E1%2586%25BA_2024-08-15_%25E1%2584%258B%25E1%2585%25A9%25E1%2584%258C%25E1%2585%25A5%25E1%2586%25AB_1.46.50.png)

Before

![After](LapTop%20UpDate%20Log/%25E1%2584%2589%25E1%2585%25B3%25E1%2584%258F%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25B5%25E1%2586%25AB%25E1%2584%2589%25E1%2585%25A3%25E1%2586%25BA_2024-09-21_%25E1%2584%258B%25E1%2585%25A9%25E1%2584%2592%25E1%2585%25AE_10.49.29.png)

After

- 2024/09/22 → `brew install luarocks`
- 2024/09/22 → `brew install lua@5.3`
- 2024/09/22 → `brew install lua-language-server`
- 2024/09/22 → `sudo npm install -g neovim`

- 2024/09/22 → `python3 -m pip install --user --upgrade pynvim`

- 2024/09/23 → `brew install tcl-tk`
- 
- 2024/09/24 → `sudo npm install -g live-server`

- 2024/09/26 → /Library/Frameworks/R.framework → `sudo rm -rf R.framework`
- 2024/09/27 → `~/.zshrc` file edit `<live-server>`**(Macbook Air first)**
    
    `alias live-server=’npx live-server’`
    
- 2024/09/29 → `brew install cloc`
- 2024/09/29 → `brew install openjdk`
- 2024/09/29 → `pip install pygame`
- 2024/09/29 → `pip3 install setuptools`

- 2024/09/30 → `pip3 install ruff`

- 2024/10/07 → `pip3 install matplotlib`
- 2024/10/07 → `pip install matplotlib`

- 2024/10/12 → Logi Options+ / Logi AI Prompt Builder **disalbed**
- 2024/10/12 → Logi Options+ / All Alarm **disalbed**
- 2024/10/13 → `pip install anthropic`
- 2024/10/13 → `pip3 install anthropic`

- 2024/10/14 → `pip install neovim`
- 2024/10/14 → `pip3 install neovim`
- 2024/10/14 → `brew install ast-grep`
- 2024/10/14 → `brew install viu`
- 2024/10/14 → `brew install chafa`
- 2024/10/14 → `~/.tmux.conf` → Moving Window Key Mapping
- tmux .conf
    
    ```lua
    if-shell 'test -z "$POWERLINE_CONFIG_COMMAND"' 'set-environment -g POWERLINE_CONFIG_COMMAND powerline-config'
    
    # Don't version-check for this core functionality -- anything too old to
    # support these options likely won't work well with powerline
    
    set-option -g focus-events on
    
    set -g status on
    set -g status-interval 2
    set -g status-left-length 70
    #set -g status-left "#(powerline tmux left)"
    #set -g status-left '#[fg=colour235,bg=colour252,bold] #S #[fg=colour252,bg=colour238,nobold]#[fg=colour245,bg=colour238,bold] #(whoami) #[fg=colour238,bg=colour234,nobold]'
    
    set -g status-right-length 150
    set -g status-right "#(powerline tmux right)"
    set -sg escape-time 0
    #set -g status-right '#[fg=colour59]#[fg=colour255,bg=colour59] #[fg=colour254,bold]#[fg=colour16,bg=colour254,bold] #h '
    
    set -g window-status-separator '#[fg=colour244,bg=colour234]'
    set -g window-status-format "#[fg=colour244,bg=colour234] #I #[fg=colour240] #[default,bg=colour234]#W "
    set -g window-status-current-format "#[fg=colour234,bg=colour31]#[fg=colour117,bg=colour31] #I  #[fg=colour231,bold]#W #[fg=colour31,bg=colour234,nobold]"
    
    # Key bind
    bind-key -n C-S-Left previous-window
    bind-key -n C-S-Right next-window
    
    # bind-key -n C-M-k select-pane -U
    # bind-key -n C-M-j select-pane -D
    # bind-key -n C-M-h select-pane -L
    # bind-key -n C-M-l select-pane -R 
    
    #Set Mouse
    set -g mouse on
    
    set -g history-limit 100000
    
    setw -g mode-keys vi
    
    # Moving Windows
    bind-key -r Left swap-window -t -1\; select-window -t -1
    bind-key -r Right swap-window -t +1\; select-window -t +1
    
    bind -r k select-pane -U
    bind -r j select-pane -D
    bind -r h select-pane -L
    bind -r l select-pane -R 
    
    # load powerline
    if-shell 'env "$POWERLINE_CONFIG_COMMAND" tmux setup' '' 'run-shell "powerline-config tmux setup"'
    
    ```
    

- 2024/10/15 → `brew install prettierd`
- 2024/10/15 → `sudo chown -R 501:20 “/Users/sangmin/.npm”`
- 2024/10/15 → `brew install kafka`

- 2024/10/16 → **Iterm2** font : **MesloLGSDZ Nerd Font**
    
    [MesloLGSDZNerdFont-Regular.ttf](LapTop%20UpDate%20Log/MesloLGSDZNerdFont-Regular.ttf)
    
- 2024/10/18 → **Iterm2** 한글 폰트 해결 → **NFC**
- 2024/10/18 → **Iterm2** Settings : Profiles/Terminal/Scrollback Buffer → **Unlimited scrollback**
- 2024/10/19 → `pip3 install setuptools`
- 2024/10/19 → **Iterm2** `General/Selection/Application in terminal may access clipboard` (checked)
    
    ![스크린샷 2024-10-19 오후 4.59.01.png](LapTop%20UpDate%20Log/%25E1%2584%2589%25E1%2585%25B3%25E1%2584%258F%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25B5%25E1%2586%25AB%25E1%2584%2589%25E1%2585%25A3%25E1%2586%25BA_2024-10-19_%25E1%2584%258B%25E1%2585%25A9%25E1%2584%2592%25E1%2585%25AE_4.59.01.png)
    

- 2024/10/26 → `brew install btop`
- 2024/10/26 → `brew install bottom`
- 2024/10/29 → `brew install  karabiner-elements`
- 2024/10/29 → `karabiner-elements` → 설정
    
    [맥(Mac) 한영 전환키 동작 빠르게 하는 방법](https://www.youtube.com/watch?v=AXuH-v1EXqs)
    
- 2024/10/29 → Dock **GitHub** 제거, **GitKraken** 추가

![Before](LapTop%20UpDate%20Log/%25E1%2584%2589%25E1%2585%25B3%25E1%2584%258F%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25B5%25E1%2586%25AB%25E1%2584%2589%25E1%2585%25A3%25E1%2586%25BA_2024-09-21_%25E1%2584%258B%25E1%2585%25A9%25E1%2584%2592%25E1%2585%25AE_10.49.29.png)

Before

![After](LapTop%20UpDate%20Log/%25E1%2584%2589%25E1%2585%25B3%25E1%2584%258F%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25B5%25E1%2586%25AB%25E1%2584%2589%25E1%2585%25A3%25E1%2586%25BA_2024-10-29_%25E1%2584%258B%25E1%2585%25A9%25E1%2584%258C%25E1%2585%25A5%25E1%2586%25AB_11.19.18.png)

After

- 2024/10/31 → `brew install zoxide`
- 2024/10/31 → `~/.zshrc` file edit `<zoxide>`
    
    ```lua
    # If you come from bash you might have to change your $PATH.
    # export PATH=$HOME/bin:/usr/local/bin:$PATH
    
    # Path to your oh-my-zsh installation.
    export ZSH="$HOME/.oh-my-zsh"
    
    # Set name of the theme to load --- if set to "random", it will
    # load a random theme each time oh-my-zsh is loaded, in which case,
    # to know which specific one was loaded, run: echo $RANDOM_THEME
    # See https://github.com/ohmyzsh/ohmyzsh/wiki/Themes
    ZSH_THEME="powerlevel10k/powerlevel10k"
    
    # Set list of themes to pick from when loading at random
    # Setting this variable when ZSH_THEME=random will cause zsh to load
    # a theme from this variable instead of looking in $ZSH/themes/
    # If set to an empty array, this variable will have no effect.
    # ZSH_THEME_RANDOM_CANDIDATES=( "robbyrussell" "agnoster" )
    
    # Uncomment the following line to use case-sensitive completion.
    # CASE_SENSITIVE="true"
    
    # Uncomment the following line to use hyphen-insensitive completion.
    # Case-sensitive completion must be off. _ and - will be interchangeable.
    # HYPHEN_INSENSITIVE="true"
    
    # Uncomment one of the following lines to change the auto-update behavior
    # zstyle ':omz:update' mode disabled  # disable automatic updates
    # zstyle ':omz:update' mode auto      # update automatically without asking
    # zstyle ':omz:update' mode reminder  # just remind me to update when it's time
    
    # Uncomment the following line to change how often to auto-update (in days).
    # zstyle ':omz:update' frequency 13
    
    # Uncomment the following line if pasting URLs and other text is messed up.
    # DISABLE_MAGIC_FUNCTIONS="true"
    
    # Uncomment the following line to disable colors in ls.
    # DISABLE_LS_COLORS="true"
    
    # Uncomment the following line to disable auto-setting terminal title.
    # DISABLE_AUTO_TITLE="true"
    
    # Uncomment the following line to enable command auto-correction.
    # ENABLE_CORRECTION="true"
    
    # Uncomment the following line to display red dots whilst waiting for completion.
    # You can also set it to another string to have that shown instead of the default red dots.
    # e.g. COMPLETION_WAITING_DOTS="%F{yellow}waiting...%f"
    # Caution: this setting can cause issues with multiline prompts in zsh < 5.7.1 (see #5765)
    # COMPLETION_WAITING_DOTS="true"
    
    # Uncomment the following line if you want to disable marking untracked files
    # under VCS as dirty. This makes repository status check for large repositories
    # much, much faster.
    # DISABLE_UNTRACKED_FILES_DIRTY="true"
    
    # Uncomment the following line if you want to change the command execution time
    # stamp shown in the history command output.
    # You can set one of the optional three formats:
    # "mm/dd/yyyy"|"dd.mm.yyyy"|"yyyy-mm-dd"
    # or set a custom format using the strftime function format specifications,
    # see 'man strftime' for details.
    # HIST_STAMPS="mm/dd/yyyy"
    
    # Would you like to use another custom folder than $ZSH/custom?
    # ZSH_CUSTOM=/path/to/new-custom-folder
    
    # Which plugins would you like to load?
    # Standard plugins can be found in $ZSH/plugins/
    # Custom plugins may be added to $ZSH_CUSTOM/plugins/
    # Example format: plugins=(rails git textmate ruby lighthouse)
    # Add wisely, as too many plugins slow down shell startup.
    plugins=(git zsh-syntax-highlighting zsh-autosuggestions autojump web-search)
    
    source $ZSH/oh-my-zsh.sh
    
    # User configuration
    
    # export MANPATH="/usr/local/man:$MANPATH"
    
    # You may need to manually set your language environment
    export LANG=en_US.UTF-8
    export LC_CTYPE=ko_KR.UTF-8  # 한글 입력을 위해 문자 인코딩을 한국어로 설정
    
    # Preferred editor for local and remote sessions
    # if [[ -n $SSH_CONNECTION ]]; then
    #   export EDITOR='vim'
    # else
    #   export EDITOR='mvim'
    # fi
    
    # Compilation flags
    # export ARCHFLAGS="-arch x86_64"
    
    # Set personal aliases, overriding those provided by oh-my-zsh libs,
    # plugins, and themes. Aliases can be placed here, though oh-my-zsh
    # users are encouraged to define aliases within the ZSH_CUSTOM folder.
    # For a full list of active aliases, run `alias`.
    #
    # Example aliases
    # alias zshconfig="mate ~/.zshrc"
    # alias ohmyzsh="mate ~/.oh-my-zsh"
    
    # To customize prompt, run `p10k configure` or edit ~/.p10k.zsh.
    
    [[ ! -f ~/.p10k.zsh ]] || source ~/.p10k.zsh
    export PATH=/opt/homebrew/bin:$PATH
    
    export PATH=$PATH:~/.npm-global/bin
    
    neofetch
    
    # alias binding
    alias cat='bat --paging never'
    alias gu='gitui'
    alias lg='lazygit'
    alias ldk='lazydocker'
    alias t='tmux'
    alias live-server='npx live-server'
    alias cd='z'
    
    eval "$(zoxide init zsh)"
    
    source /Users/sangmin/.config/broot/launcher/bash/br
    
    ```
    
- 2024/10/31 → `brew install dust`
- 2024/10/31 → `brew install duf`
- 2024/10/31 → `brew install jq`
- 2024/10/31 → `brew install procs`
- 2024/10/31 → `brew install git-delta`
- 2024/10/31 → `~/.gitconfig` file edit `<git-delta>`
    
    ```lua
    [user]
    	email = sm010422@naver.com
    	name = Park Sang Min
    [core]
    	excludesfile = /Users/sangmin/.gitignore_global
      pager = delta
    [difftool "sourcetree"]
    	cmd = opendiff \"$LOCAL\" \"$REMOTE\"
    	path = 
    [mergetool "sourcetree"]
    	cmd = /Applications/Sourcetree.app/Contents/Resources/opendiff-w.sh \"$LOCAL\" \"$REMOTE\" -ancestor \"$BASE\" -merge \"$MERGED\"
    	trustExitCode = true
    [commit]
    	template = /Users/sangmin/.stCommitMsg
    [filter "lfs"]
    	clean = git-lfs clean -- %f
    	smudge = git-lfs smudge -- %f
    	process = git-lfs filter-process
    	required = true
    [credential]
    	helper = osxkeychain
    [push]
    	autoSetupRemote = true
    
    [interactive]
        diffFilter = delta --color-only
    
    [delta]
        navigate = true    # use n and N to move between diff sections
    
        # delta detects terminal colors automatically; set one of these to disable auto-detection
        # dark = true
        # light = true
    
    [merge]
        conflictstyle = zdiff3
    
    ```
    
- 2024/10/31 → `brew install gping`
- 2024/10/31 → `brew install broot`
- 2024/10/31 → `~/.config/broot/verb.hjson` → **key** & **execution** edit

- 2025/01/18 → `sudo npm install -g markdown-toc`
- 2025/01/18 → `sudo npm install -g markdownlint-cli2`
- 2025/01/18 → `sudo npm install -g prettier`
- 2025/01/18 → `pip install sqlfluff`
- 2025/01/18 → `brew install prettier`
- 2025/01/18 → `brew install cmake`
- 2025/01/18 → `brew install libvips`
- 2024/11/05 → `brew install tbb`
- 2024/11/05 → `brew install libxcb`
    
    pkg-config --modversion xcb-image 명령을 실행했을 때 “Package xcb-image was not found”라는 메시지가 뜨는 것은 xcb-image 패키지가 시스템에 설치되지 않았거나, pkg-config가 해당 패키지를 찾을 수 있는 경로에 없다는 것을 의미합니다. 이 문제를 해결하기 위해 다음 단계를 따라 해보세요:
    
    **1. xcb-image 설치 확인**
    
    xcb-image는 일반적으로 libxcb 라이브러리의 일부로 설치됩니다. 먼저 libxcb가 설치되어 있는지 확인합니다:
    
    brew list libxcb
    
    이 명령어가 libxcb의 설치 파일 목록을 반환하면 이미 설치된 것입니다. 그렇지 않다면, 아래 명령어로 설치합니다:
    
    brew install libxcb
    
    **2. xcb-util 및 관련 패키지 설치**
    
    xcb-image는 xcb-util 패키지와 관련이 있을 수 있습니다. 이 패키지를 설치하면 필요한 라이브러리를 포함할 수 있습니다:
    
    brew install xcb-util
    
    또한, xcb-util-image 패키지를 설치해보세요:
    
    brew install xcb-util-image
    
    **3. 환경 변수 설정**
    
    PKG_CONFIG_PATH에 pkg-config가 xcb-image.pc 파일을 찾을 수 있도록 설정해주어야 할 수도 있습니다. 일반적으로 Homebrew가 설치한 패키지의 .pc 파일은 /opt/homebrew/lib/pkgconfig에 있습니다. 해당 경로를 PKG_CONFIG_PATH에 추가합니다.
    
    export PKG_CONFIG_PATH=/opt/homebrew/lib/pkgconfig:$PKG_CONFIG_PATH
    
    이 설정을 셸의 초기화 파일 (예: ~/.bashrc, ~/.zshrc)에 추가하여 항상 적용될 수 있도록 합니다.
    
    **4. 재시도**
    
    위의 단계를 완료한 후, 다음 명령어로 xcb-image가 제대로 설치되었는지 확인합니다:
    
    pkg-config --modversion xcb-image
    
    이제 CMake를 다시 실행해 보세요:
    
    cmake .
    
    이렇게 해도 문제가 해결되지 않으면, 추가적으로 CMakeLists.txt 파일에서 직접 의존성을 확인하고 조정해야 할 수도 있습니다.
    
- 2024/11/05 → `brew install opencv`
- 2024/11/05 → `brew install llvm`
- 2024/11/05 → `brew install nlohmann-json`
- 2024/11/05 → `brew install cli11`

- 2024/11/06 → `brew install perl`
- 2024/11/08 → 설정/키보드/키보드 단축키/Launchpad 및 Dock → Dock 가리기 켜기/끄기 `off`
- 2024/11/10 → 설정/키보드/키보드 단축키/Spotlight → Spotlight 검색 보기 `off`

- 2024/11/11 → `pip install debugpy`
- 2024/11/11 → `brew install mercurial`
- 2024/11/11 → `brew install libxres`
- 2024/11/11 → `brew install jstkdng/programs/ueberzugpp`

- 2024/11/21 → **Iterm2** Settings : Profiles/Session/Status bar enabled → **Off**

- 2024/11/25 → **Magnet** Settins : Hide menu bar icon → **On**

- 2024/11/26 → `brew install awscli`

- 2024/12/02 → **GitHub Desktop** app Dlete
- 2024/12/05 → **ChatGTP App** : 설정 / 앱 /  ChatGPT 보기 : Dock 및 메뉴바 → **Dock에만**
- 2024/12/05 → 설정 / 제어센터 / 메뉴 막대만 / **Spotlight** : 메뉴 막대에서 보기 → **메뉴 막대에서 보지 않음**
- 2024/12/05 → 설정 / 제어센터 / 제어 센터 모듈 / **지금 재생 중** : 활성화 상태일 때 보기 → **메뉴 막대에서 보지 않음**
- 2024/12/05 → 설정 / 제어센터 / 제어 센터 모듈 / **사운드** : 활성화 상태일 때 보기 → **메뉴 막대에서 보지 않음**
    - 2024/12/05 → **Notion** 메뉴바 → 메뉴 모음에 Notion 표시 → **Off**

- 2024/12/07 → 설정 / 데스크탑 및 Dock / **핫코너** → **모두 비활성화**
    
    ![스크린샷 2024-12-07 오전 2.17.07.png](LapTop%20UpDate%20Log/%25E1%2584%2589%25E1%2585%25B3%25E1%2584%258F%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25B5%25E1%2586%25AB%25E1%2584%2589%25E1%2585%25A3%25E1%2586%25BA_2024-12-07_%25E1%2584%258B%25E1%2585%25A9%25E1%2584%258C%25E1%2585%25A5%25E1%2586%25AB_2.17.07.png)
    
- 2024/12/07 → 설정 / 데스크탑 및 Dock / **스테이지 매니저에서 최근 사용합 앱 보기** → **Off**

- 2024/12/09 → `brew install fastfetch`
    
    [Willem Zesenzestig](https://www.facebook.com/photo/?fbid=10219918103342096&set=gm.25674946305453809&idorvanity=2735164529858645)
    

- 2024/12/20 → `brew install atuin`
    
    [Getting started](https://docs.atuin.sh/)
    
- 2024/12/20 → `brew install direnv`
    
    [direnv – unclutter your .profile](https://direnv.net/)
    
- 2024/12/20 → `brew uninstall eza`
    
    ```bash
    alias ll="eza -al --icons --git --group-directories-first --time-style=iso --binary"
    
    ```
    
    [https://github.com/eza-community/eza](https://github.com/eza-community/eza)
    
- 2024/12/20 → `brew install ranger`
    
    [https://github.com/ranger/ranger](https://github.com/ranger/ranger)
    
- 2024/12/20 → `brew install zsh-autosuggestions`

- 2024/12/28 → **Spring** initalizr App install
    
    [start.spring.io](https://start.spring.io/)
    
- 2024/12/29 → `brew install gradle`
- 2024/12/29 → **Sublime Text** App delete by **AppCleaner**

![스크린샷 2025-01-18 오후 5.21.46.png](LapTop%20UpDate%20Log/%25E1%2584%2589%25E1%2585%25B3%25E1%2584%258F%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25B5%25E1%2586%25AB%25E1%2584%2589%25E1%2585%25A3%25E1%2586%25BA_2025-01-18_%25E1%2584%258B%25E1%2585%25A9%25E1%2584%2592%25E1%2585%25AE_5.21.46.png)

- 2025/01/06 → `brew install tmux-xpanes`
- 2025/01/07 → `brew install tldr`
- 2025/01/07 → `brew reinstall docker`
- 2025/01/07 → `brew install docker-completion`
- 2025/01/07 → `brew install go`
- 2025/01/07 → `brew install go-md2man`
- 2025/01/07 → `brew install lima`
- 2025/01/07 → `brew install colima`

- 2025/01/08 → `brew install yazi`
- 2025/01/08 → `brew uninstall ranger`
- 2025/01/08 → `brew install saulpw/vd/visidata`
- 2025/01/08 → `brew tap jorgerojas26/lazysql` && `brew install lazysql`
- 2025/01/08 → `brew install mycli`

- 2025/06/20 → MacBook Pro Language Change **Korea → English**
- 2025/06/20 → `brew install qemu`

- 2025/04/14 → Dock **IntelliJ**, **PyCharm**, **CLion**, **DataGrip**, **VMware** remove

![Screenshot 2025-04-14 at 10.33.31 PM.png](LapTop%20UpDate%20Log/Screenshot_2025-04-14_at_10.33.31_PM.png)

- 2025/06/20 → **Memory Diag** key Binding → `command + shift + m` : Recycle Shortcuts

- 2025/04/22 → Dock **VSCode** remove
    
    ![Screenshot 2025-04-22 at 12.48.25 AM.png](LapTop%20UpDate%20Log/Screenshot_2025-04-22_at_12.48.25_AM.png)
    
- 2025/04/22 → Dock **Notion Calender** reorder
    
    ![Screenshot 2025-04-22 at 12.49.57 AM.png](LapTop%20UpDate%20Log/Screenshot_2025-04-22_at_12.49.57_AM.png)
    

- 2025/06/20 → `brew install doxygen`
- 2025/06/20 → `brew intstall java11`
- 2025/06/20 → `brew tap spring-io/tap` / `brew install spring-boot`
    
    [Installing Spring Boot :: Spring Boot](https://docs.spring.io/spring-boot/installing.html#getting-started.installing.cli)
    
- 2025/06/20 → `npm install -g dockerfile-language-server-nodejs`
- 2025/06/20 → `brew install dockerfile-language-server`

- 2025/06/20 → `brew install postgresql`

- 2025/06/20 → Dock **IntelliJ, DataGrip setting**
    
    ![Screenshot 2025-05-25 at 2.36.54 PM.png](LapTop%20UpDate%20Log/Screenshot_2025-05-25_at_2.36.54_PM.png)
    
- 2025/06/20 → **iterm2** Settings : Profiles/Colors/Context-aware cursor color (affects box cursor only) → Uncheck & Cursor Color change
    - Background: #ffffff (White)
    - Foreground: #000000 (Black)
    
    ![Screenshot 2025-05-26 at 5.57.11 PM.png](LapTop%20UpDate%20Log/Screenshot_2025-05-26_at_5.57.11_PM.png)
    
- 2025/06/20 → `brew install lima-additional-guestagents`
- 2025/06/20 → `npm config set prefix ~/.npm-global`
- 2025/06/20 → `npm install -g vscode-langservers-extracted`
- 2025/06/20 → `npm install -g dockerfile-language-server-nodejs`
- 2025/06/20 → `brew install marksman`
- 2025/06/20 → `brew install wakatime-cli`

- 2025/06/23 → Dock Docker Desktop add;
    
    ![Screenshot 2025-06-23 at 11.35.52 PM.png](LapTop%20UpDate%20Log/Screenshot_2025-06-23_at_11.35.52_PM.png)
    
- 2025/06/23 → `brew install jenkins`
- 2025/06/23 → `brew install jenkins-cli`

- 2025/06/17 → `brew uninstall atuin` & ./zshrc `eval “$(atuin init zsh)”` → comment
- 2025/06/30 → MySQL WorkBench : Dock removed
- 2025/07/01 → `brew install scc`

- 2025/07/01 → `brew uninstall cloc`
- 2025/07/01 → Dock Update : **Postman** add
    
    ![Screenshot 2025-07-01 at 11.17.02 PM.png](LapTop%20UpDate%20Log/Screenshot_2025-07-01_at_11.17.02_PM.png)
    

- 2025/07/08 → `brew install --cask hammerspoon`
- 2025/07/08 → **hammerspoon init.lua** config
    
    ```bash
    mkdir ~/.hammerspoon
    touch ~/.hammerspoon/init.lua
    
    open ~/.hammerspoon/init.lua
    ```
    
    ```lua
    local function switchToEnglish()
      -- 영어 입력기의 ID: ABC는 "com.apple.keylayout.ABC"
      hs.keycodes.currentSourceID("com.apple.keylayout.ABC")
    end
    
    -- 앱 변경 감지
    appWatcher = hs.application.watcher.new(function(appName, eventType, appObject)
      if eventType == hs.application.watcher.activated then
        if appName == "iTerm2" then
          switchToEnglish()
        end
      end
    end)
    
    appWatcher:start()
    			
    ```
    
    ![Screenshot 2025-07-08 at 10.28.05 AM.png](LapTop%20UpDate%20Log/Screenshot_2025-07-08_at_10.28.05_AM.png)
    
    ![Screenshot 2025-07-08 at 10.29.19 AM.png](LapTop%20UpDate%20Log/Screenshot_2025-07-08_at_10.29.19_AM.png)
    
    ![스크린샷 설명](laptop/Screenshot_202025-07-08_at_10.27.34_AM.png)
    

- 2025/07/09 → `brew install jenv`   & .zshrc code add
    
    ```bash
    #java jenv setting
    export PATH="$HOME/.jenv/bin:$PATH"
    eval "$(jenv init -)"
    
    ```
    
- 2025/07/10 → `brew install --cask sublime-text`
- 2025/07/10 →
    
    ```bash
    brew uninstall mysql
    brew install mysql@8.0
    brew link --force mysql@8.0
    ```
    
- 2025/07/22 → `brew install nginx`
- 2025/07/23 → `npm install -g pm2`
- 2025/07/28 → `brew install --cask claude`
- 2025/07/30 → `brew install google-java-format`
- 2025/07/30 → `sudo npm install -g @google/gemini-cli`
- 2025/08/04 → `brew install redis`
- 2025/08/05 → `brew install --cask redis-insight`
- 2025/08/06 → `brew install iredis`

- 2025/08/18 → `brew install lnav`
- 2025/08/21 → `brew install dive`
- 2025/08/21 → Dock Update : **Redis Insight** add
    
    ![Screenshot 2025-08-21 at 5.34.27 PM.png](LapTop%20UpDate%20Log/Screenshot_2025-08-21_at_5.34.27_PM.png)
    
- 2025/08/22 → PinPoint :
    - wget [https://github.com/pinpoint-apm/pinpoint/releases/download/v2.5.3/pinpoint-agent-2.5.3.tar.gz](https://github.com/pinpoint-apm/pinpoint/releases/download/v2.5.3/pinpoint-agent-2.5.3.tar.gz)
    
- 2025/09/01 → **CLion** remove by **AppCleaner**
- 2025/09/04 → `jenv add "$(/usr/libexec/java_home -v 21)”`
- 2025/09/04 → `jenv global 21.0.1`
- 2025/09/04 → `jenv enable-plugin export`
    
    [[Setting] jenv로 여러 Java 버전 사용/관리하기 (For Mac)](https://velog.io/@geun/Setting-jenv%EB%A1%9C-%EC%97%AC%EB%9F%AC-Java-%EB%B2%84%EC%A0%84-%EC%82%AC%EC%9A%A9%EA%B4%80%EB%A6%AC%ED%95%98%EA%B8%B0-For-Mac-g20bsd7e)
    
- 2025/09/09 → `brew install k6`
- 2025/09/11 → `brew install mysql-client`
- 2025/09/15 → `brew install openssh`
- 2025/09/29 → Dock Update : **ChatGPT** remove
    
    ![Screenshot 2025-09-29 at 9.47.26 AM.png](LapTop%20UpDate%20Log/Screenshot_2025-09-29_at_9.47.26_AM.png)
    

- 2025/10/28 → `brew install coursier/formulas/coursier`
    
    [Installation · Coursier](https://get-coursier.io/docs/cli-installation)
    
- 2025/10/28 → `cs setup`
- 2025/11/13 → `brew install posting`
- 2025/11/13 → `pip3 install pydantic`
- 2025/11/13 → `/opt/homebrew/Cellar/posting/2.9.2/libexec/bin/python3.14 -m pip install pydantic`
- 2025/11/20 → `brew install bandwhich`
- 2025/11/25 → `brew install hadoop`

---

# Bottom
