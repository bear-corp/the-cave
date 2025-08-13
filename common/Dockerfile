FROM mcr.microsoft.com/devcontainers/base:ubuntu

USER vscode

#### 🎨 ZSH & OhMyZsh configuration 🖥️  ####
ENV ZSH_CUSTOM=/home/vscode/.oh-my-zsh/custom
COPY .zshrc /home/vscode/.zshrc
RUN git clone https://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
RUN git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
RUN ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"