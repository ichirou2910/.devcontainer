# Ichirou's Devcontainer config

## Usage

- Copy config from targeted framework to your project root
- Edit network name if needed
- Edit port and service name in `devcontainer.json`

```json
{
  "runArgs": ["--name=service-frontend", "-p=5000:5000"]
}
```

## General

### Features

- Neovim: terminal text editor, Nightly build
- nnn: terminal file explorer, latest version build
- fzf: fuzzy finder
- ripgrep: text search
- exa: ls replacement

### Other

- Join the same docker network to enable communication between containers
- Set default shell to ZSH
  - ZSH config file at `$HOME/.config/zsh`

## Frameworks

### .NET

- .NET 6.0: for project
- .NET 8.0: for C# LSP

### React

- Node 18 + TypeScript
