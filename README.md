# local-config
Basic everyday software for configuring my local machine

## Tooling

- [Homebrew](https://brew.sh/)
- [powerlevel10k](https://github.com/romkatv/powerlevel10k)

## How to install tooling

1. Configure a terminal (usually [iterm2](https://iterm2.com/)]
2. Install [powerlevel10k](https://github.com/romkatv/powerlevel10k)
3. Install [Homebrew](https://brew.sh/)
4. Run `$ brew bundle install --file=Brewfile --cleanup --zap`

## Useful

1. For quick access and avoiding conflicts, consider adding this shortcut to the `.zshrc`

```
local-config() {
  cd local-config && git pull -r
}
```
