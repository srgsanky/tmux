# tmux configuration

prefix is `<C-b>` (ctrl+b).

## Install latest tmux

Make sure you have tmux 3.5. Use `tmux -V` to list the version. If you have an older version, build and install the
latest tmux.

```bash
sudo yum install -y libevent-devel ncurses-devel ncurses-libs

git clone https://github.com/tmux/tmux.git
cd tmux
sh autogen.sh
./configure --prefix=/usr && make -j && sudo make install
```

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

## Plugin management

Remove unused plugins

```bash
~/.config/tmux/plugins/tpm/bin/clean_plugins
```
