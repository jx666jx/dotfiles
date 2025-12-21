# dotfiles setup
- install chezmoi and dotfiles

    ```sh -c "$(curl -fsLS get.chezmoi.io)" -- init --apply https://github.com/jx666jx/dotfiles```
- install dotfiles with cehzmoi but remove chezmoi when done

    ```sh -c "$(curl -fsLS get.chezmoi.io)" -- init --one-shot https://github.com/jx666jx/dotfiles```

# tools

install these tools before cloning the dotfiles

## install linux default repo stuff
```sudo apt install curl dnsutils fonts-powerline git htop jq netcat-traditional nmap zsh```

## install oh-my-zsh
```sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"```

oh-my-zsh auto-suggestions

```git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/zsh-autosuggestions```

oh-my-zsh powerlevel10k theme

```git clone --depth=1 https://github.com/romkatv/powerlevel10k.git "${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k"```

## install VSCode
- arm 

```https://code.visualstudio.com/docs/?dv=linuxarm64_deb```
- X64

```https://code.visualstudio.com/docs/?dv=linux64_deb```


## copy these binaries to ~/.local/bin
- bat 
    
    ```https://github.com/sharkdp/bat/releases```
- chezmoi 
    
    ```https://github.com/twpayne/chezmoi/releases```
- fzf 
    
    ```https://github.com/junegunn/fzf/releases```
- gh

    ```https://github.com/cli/cli/releases```
- glab

    ```https://gitlab.com/gitlab-org/cli/-/releases```


- ripgrep 
    
    ```https://github.com/BurntSushi/ripgrep/releases```
- kubectl
    - Grab the latest version for platform. (update the url for amd or arm)
    
        ```curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/{amd64|arm64}/kubectl"```

    - Directly download a specific version and platform.
        
        ```curl -LO https://dl.k8s.io/release/v1.35.0/bin/linux/arm64/kubectl```
- kubectx / kubens
    
    ```https://github.com/ahmetb/kubectx/releases```
- k9s
    
    ```https://github.com/derailed/k9s/releases```
