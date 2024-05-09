# tmux configuration

prefix is `<C-b>` (ctrl+b).

## Initial setup

```bash
# Clone Tmux Plugin Manager (tpm).
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

mkdir -p ~/.config/
git clone https://github.com/srgsanky/tmux ~/.config/tmux
```

Once in tmux, install plugins using `<prefix> I` (To update plugins use `<prefix> U`)

## Updates to tmux.conf

After editing tmux.conf, reload it using

```bash
tmux source ~/.config/tmux/tmux.conf
```
