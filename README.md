# kde-dotfiles

![Screenshot](../master/screenshots/screenshot-1.png)

## Dependencies
### Konsave
This package is necessary to import this KDE theme, it can be installed from the [AUR](https://aur.archlinux.org/packages/konsave) using yay
```bash
yay -Sy konsave
```
Or using
```bash
git clone https://aur.archlinux.org/konsave.git
cd konsave
makepkg -sic
```

### ttf-font-awesome
```bash
sudo pacman -S ttf-font-awesome
```
## Optional 
[capitaine-cursors](https://github.com/keeferrourke/capitaine-cursors) and [papirus-icon-theme](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme) 
```bash
sudo pacman -S capitaine-cursors papirus-icon-theme 
```

## Apply the theme

```bash
git clone https://github.com/amineboucenna/kde-dotfiles.git
cd kde-dotfiles/
cp -r konsave/ ~/.config
konsave -a kde-dotfiles
```

Restart KDE by making logout or using this command

```bash
killall plasmashell; kstart plasmashell
```
