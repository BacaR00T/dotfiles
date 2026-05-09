# dotfiles

## clone

```bash
git clone https://github.com/BacaR00T/dotfiles
cd ~/dotfiles
yay -S alacritty dmenu input-remapper polkit-gnome brave-bin thunar feh picom fish stow i3status-rust gvfs gvfs-smb smbclient cifs-utils

stow
stow -t ~ alacritty fish i3 i3status-rust extras

unstow
stow -t ~ -D alacritty fish i3 i3status-rust extras

restow
stow -t ~ -R alacritty fish i3 i3status-rust extras
```

![literally me](lain.png)
