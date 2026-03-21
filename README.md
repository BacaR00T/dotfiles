# dotfiles (i3 + X11)

Fresh install → run one script → i3 setup + my configs.

## Use

```bash
# install git (pick one)
sudo pacman -S git        # Arch
sudo apt install git      # Debian/Ubuntu
sudo dnf install git      # Fedora
sudo xbps-install -S git  # Void

git clone https://github.com/BacaR00T/i3wm-config- dotfiles
cd dotfiles
chmod +x bootstrap.sh
./bootstrap.sh
````

## What it does (depending on checklist)

* installs i3 stuff: i3status / i3lock / xss-lock / dex / nm-applet / polkit / picom / feh
* installs apps: alacritty / dmenu / thunar
* installs + sets default shell: fish
* installs + enables display manager: ly (best effort on some distros)
* copies configs from `./home` to `~` (backs up existing files)
* creates `~/.xsession` (so ly can start i3)

## Layout

`home/` mirrors `$HOME`:

```
home/
  .config/i3/config
  .config/alacritty/alacritty.toml
  .config/picom/picom.conf
  .config/i3status/config
  .config/fish/config.fish
  .local/bin/browser
```
