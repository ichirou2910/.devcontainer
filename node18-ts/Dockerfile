FROM mcr.microsoft.com/devcontainers/typescript-node:1-18-bookworm

RUN chsh -s /usr/bin/zsh node

RUN echo 'export ZDOTDIR=$HOME/.config/zsh' >> /home/node/.zshenv

CMD [ "zsh" ]
