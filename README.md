# local-config
Basic everyday software for configuring my local machine

## Tooling

- [Homebrew](https://brew.sh/)
- [powerlevel10k](https://github.com/romkatv/powerlevel10k)

## How to install tooling

1. Install [Homebrew](https://brew.sh/)
2. Run `$ brew bundle install --file=Brewfile --cleanup --zap`
3. Configure [ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)
4. Configure [powerlevel10k](https://github.com/romkatv/powerlevel10k)

### Suggested ohmyzsh plugins

``` text
plugins=(
  zsh-autosuggestions
  git
  gradle
  safe-paste
  brew
  docker
  docker-compose
  kubectl
  kubectx
  helm
  terraform
  aws
)
```

## Useful

1. For quick access and avoiding conflicts, consider adding this shortcut to the `.zshrc`

```
local-config() {
  cd local-config && git pull -r && brew bundle install --file=Brewfile --cleanup --zap
}
```
