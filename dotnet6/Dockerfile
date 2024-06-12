FROM mcr.microsoft.com/devcontainers/dotnet:1-6.0-bullseye

RUN apt-get update && apt-get install -y gss-ntlmssp

RUN wget https://dot.net/v1/dotnet-install.sh \
    && chmod +x dotnet-install.sh

RUN ./dotnet-install.sh --install-dir /usr/share/dotnet --channel 8.0

RUN dotnet workload update

RUN chsh -s /usr/bin/zsh vscode

RUN echo 'export ZDOTDIR=$HOME/.config/zsh' >> /home/vscode/.zshenv

CMD [ "zsh" ]
