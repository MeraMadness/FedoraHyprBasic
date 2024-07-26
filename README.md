# FedoraHypr - Basic Hyprland Config for Fedora.

This was from YT video, is not an incredible rice, just a starting point.

If you want a videoguide, just go to my YT channel • [MeraMadness](https://www.youtube.com/watch?v=jT6yYftI79g&lc=UgyE4DIoUl7Lln8qonZ4AaABAg)

I did a minimal install of Fedora 40 using the Fedora Everything ISO [LINK](https://alt.fedoraproject.org/en/)

What you need? - Time, a bit of patience and a lot of dependencies.

- **Window Manager** • [Hyprland](https://wiki.hyprland.org/) 
- **Terminal** • [Kitty](https://sw.kovidgoyal.net/kitty/#)
- **Bar** • [Waybar](https://github.com/Alexays/Waybar)
- **Notify Daemon** • [dunst](https://github.com/dunst-project/dunst)
- **Lock** • [Hyprlock](https://github.com/hyprwm/hyprlock/)
- **Apps Launcher** • [Rofi-Wayland](https://github.com/lbonn/rofi)
- **Wallpaper Selector** • [Hyprpaper](https://github.com/hyprwm/hyprpaper)
- **File Manager** • [Dolphin](https://github.com/KDE/dolphin)
- **LoginCTL** • [Wlogout](https://github.com/ArtsyMacaw/wlogout)
- **Wayland Clipboard** • [cliphist](https://github.com/sentriz/cliphist)
- **Screenshot Utility** • [grim](https://github.com/emersion/grim) - [slurp](https://github.com/emersion/slurp)
- **Fetch** • [Fastfetch](https://github.com/fastfetch-cli/fastfetch)
- **GTK Theme Selector** • [NWG-Look](https://github.com/nwg-piotr/nwg-look)
- **QT Theme Selector** • [Kvantum](https://github.com/tsujan/Kvantum/blob/master/Kvantum/INSTALL.md) | [qt6ct](https://github.com/trialuser02/qt6ct)

Themes and Icon I use.
- **Materia-GTK** • [Materia-GTK](https://github.com/nana-4/materia-theme)
- **Materia-KDE** • [Materia-KDE](https://github.com/PapirusDevelopmentTeam/materia-kde)
- **Tela Circle** • [Tela](https://github.com/vinceliuice/Tela-circle-icon-theme)

## ⛧ Images

<img align="center" src="/img/Simple.webp">

### Install Steps

<details>

<summary><b>Disclaimer</b></summary>

## Installation

##### This guide is just for Fedora, but if you install every Dependencies, you can use it on every distro.

<div align="left">

<details>
<summary><h3> Hyprland and other stuff from the Fedora Repo<h3></summary>

###### Just install Hyprland from the Fedora Repo using dnf.

```sh
### Hyprland and other stuff
paru -S hyprland waybar wlogout kitty rofi-wayland qt6ct kvantum dolphin polkit-gnome ### Fedora Repo has everything.
```

</details>

<details>
<summary><h3>Hyprland Eco System</h3></summary>

###### We need the Solopasha COPR, this Repo has everything about Hyprland.

```sh
### Hyprland apps
Enable the Repo - sudo dnf copr enable solopasha/hyprland
then Install - sudo dnf hyprpaper cliphist hyprlock 
```
<details>
<summary><h3>Dotfiles</h3></summary>

```sh
# Dotfiles
git clone https://github.com/MeraMadness/FedoraHyprBasic.git $HOME/Downloads/FedoraHyprBasic/
cd $HOME/Downloads/FedoraHyprBasic
cp -r .config/* $HOME/.config
cp -r .cache/* $HOME/.cache

</details>

</div>

