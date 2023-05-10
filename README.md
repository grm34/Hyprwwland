# Hyprwwland

A simple sharing of my Eww setup on Hyprland to serve as an example or basis for learning how to create your own desktop environment. Many thanks to [@ElKowar](https://github.com/elkowar) for this awesome standalone widget system made in Rust. To be used without moderation.

<a href="https://raw.githubusercontent.com/grm34/Hyprwwland/main/assets/screenshots/screen1.png">
  <img align="center" width="49%" src="assets/screenshots/screen1.png"/>
</a>
<a href="https://raw.githubusercontent.com/grm34/Hyprwwland/main/assets/screenshots/screen2.png">
  <img align="center" width="49%" src="assets/screenshots/screen2.png"/>
</a>
<a href="https://raw.githubusercontent.com/grm34/Hyprwwland/main/assets/screenshots/screen3.png">
  <img align="center" width="49%" src="assets/screenshots/screen3.png"/>
</a>
<a href="https://raw.githubusercontent.com/grm34/Hyprwwland/main/assets/screenshots/screen4.png">
  <img align="center" width="49%" src="assets/screenshots/screen4.png"/>
</a>

https://github.com/grm34/Hyprwwland/assets/6394023/36422967-54ce-401f-bd17-5b7e22b8be2d

In order to keep this clean, and being only an Eww configuration, my dotfiles are on a separate repository [Hyprwwland-dotfiles](https://github.com/grm34/Hyprwwland-dotfiles).

## What I use

- **Distro** : [Arch Linux](https://wiki.archlinux.org)
- **AUR Helper** : [paru-git](https://github.com/Morganamilo/paru)
- **Display Server** : [wayland](https://wayland.freedesktop.org/docs/html)
- **Window Manager** : [hyprland](https://wiki.hyprland.org)
- **Desktop Widgets** : [eww-wayland](https://elkowar.github.io/eww)
- **Notifications** : [dunst](https://github.com/dunst-project/dunst) [libnotify](https://gitlab.gnome.org/GNOME/libnotify)
- **Lock Screen** : [swayidle](https://github.com/swaywm/swayidle) [swaylock-effects-git](https://github.com/mortie/swaylock-effects)
- **Wallpaper Manager** : [hyprpaper](https://github.com/hyprwm/hyprpaper)
- **System Clipboard** : [wl-clipboard](https://github.com/bugaevc/wl-clipboard) [cliphist](https://github.com/sentriz/cliphist)
- **Sound system** : [pipewire](https://docs.pipewire.org) [wireplumber](https://gitlab.freedesktop.org/pipewire/wireplumber) [pulsemixer](https://github.com/GeorgeFilipkin/pulsemixer)
- **Brightness Control** : [light](https://haikarainen.github.io/light)
- **App Launcher** : [fuzzel](https://codeberg.org/dnkl/fuzzel)
- **File Manager** : [felix-rs](https://kyoheiu.dev/felix)
- **Network** : [networkmanager](https://www.networkmanager.dev) 
- **VPN** : [wireguard-tools](https://git.zx2c4.com/wireguard-tools)
- **Multimedia Support** : [gstreamer](https://gitlab.freedesktop.org/gstreamer/gstreamer) [ffmpeg](https://ffmpeg.org) [vlc](https://www.videolan.org/vlc)
- **System info** :  [neofetch](https://github.com/dylanaraps/neofetch) [duf](https://github.com/muesli/duf) [macchina](https://github.com/Macchina-CLI/macchina)
- **Monitoring** : [btop](https://github.com/aristocratos/btop) [htop](https://github.com/htop-dev/htop) [bandwhich](https://github.com/imsnif/bandwhich)
- **Terminal** : [alacritty](https://alacritty.org) [zellij](https://zellij.dev)
- **Shell** : [nushell](https://www.nushell.sh)
- **Prompt** : [starship](https://starship.rs) [zoxide](https://github.com/ajeetdsouza/zoxide)
- **Browser** : [librewolf-bin](https://librewolf.net)
- **Screenshots** : [hyprshot](https://github.com/Gustash/hyprshot) [grim](https://wayland.emersion.fr/grim) [slurp](https://wayland.emersion.fr/slurp)
- **Screen Recorder** : [wayfarer](https://github.com/stronnag/wayfarer)
- **Text Editor** : [helix](https://helix-editor.com)
- **Terminal Pager** : [bat](https://github.com/sharkdp/bat) [less](https://greenwoodsoftware.com/less) [most](https://www.jedsoft.org/most) [git-delta](https://github.com/dandavison/delta)
- **Image Viewer** : [feh](https://github.com/derf/feh) [chafa](https://github.com/hpjansson/chafa)
- **Image Editor** : [imagemagick](https://github.com/ImageMagick/ImageMagick) [gimp](https://www.gimp.org)
- **Color Picker** : [hyprpicker](https://github.com/hyprwm/hyprpicker)
- **Document Viewer** : [zathura](https://git.pwmt.org/pwmt/zathura) [zathura-pdf-mupf](https://git.pwmt.org/pwmt/zathura-pdf-mupdf)
- **Fonts** : [Nerd Fonts](https://www.nerdfonts.com)
- **Themes** : [breeze-gtk](https://invent.kde.org/plasma/breeze-gtk) [adwaita-qt5](https://github.com/FedoraQt/adwaita-qt) [adwaita-qt6](https://github.com/FedoraQt/adwaita-qt)
- **Cursors** : [capitaine-cursors](https://github.com/keeferrourke/capitaine-cursors)
- **Icons** : [papirus-icon-theme](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme)
- **Xmpp Client** : [gajim-git](https://gajim.org)
- **GUI Settings Editor** : [nwg-look-bin](https://github.com/nwg-piotr/nwg-look) [qt5ct](https://sourceforge.net/projects/qt5ct) [qt6ct](https://github.com/trialuser02/qt6ct)
- **Desktop Portal** : [xdg-desktop-portal-hyprland](https://github.com/hyprwm/xdg-desktop-portal-hyprland)

## Quick Install on Arch Linux

- Install Eww with Hyprland and minimum requirements :

```bash
paru --needed -S hyprland eww-wayland dunst libnotify libcanberra\
                 hyprpaper swayidle swaylock-effects-git neofetch duf\
                 wl-clipboard cliphist pulsemixer light jq networkmanager\
                 sound-theme-freedesktop
```

- Install required fonts :

```bash
paru --needed -S ttf-anonymouspro-nerd ttf-jetbrains-mono-nerd\
                 ttf-ubuntu-nerd ttf-meslo-nerd papirus-icon-theme
```

- Clone the repository in your `$HOME` config folder :

```bash
git clone https://github.com/grm34/Hyprwwland "$HOME/.config/eww"
```

## Configuring

The config is located in `~/.config/eww/config.json`.
Add at least your terminal, web browser and file manager. 

```json
"aur_helper": "paru",
"terminal": "alacritty",
"terminal_cmd": "alacritty -e",
"web_browser": "librewolf",
"file_manager": "alacritty -e felix",
"sound_manager": "alacritty -e pulsemixer",
"suspend_timeout": "300",
"sleep_timeout": "600",
"weather_location": "Montpellier",
"launcher_app_path": "/usr/share/applications",
"launcher_app_icon_path": "/usr/share/icons/ePapirus-Dark/96x96/apps",
"dock_app_path": "/usr/share/applications",
"dock_app_icon_path": "/usr/share/icons/ePapirus-Dark/96x96/apps",
"dock_app_icon_size": "38"
```

To be notified of new updates allow `paru` to be runned without password in `~/etc/sudoers` :

```bash
<username> ALL=(ALL) NOPASSWD: /usr/bin/paru
```

## Auto-start with Hyprland

- Edit `~/.config/hypr/hyprland.conf` :

```text
exec-once = wl-paste --type text --watch cliphist store
exec-once = wl-paste --type image --watch cliphist store
exec-once = dunst
exec-once = hyprpaper
exec-once = eww open-many topbar dock
```

- Create `~/.config/hypr/hyprpaper.conf` :

```text
preload = ~/.config/eww/assets/wallpapers/od_neon.png
preload = ~/.config/eww/assets/wallpapers/od_shards.png
wallpaper = ~/.config/eww/assets/wallpapers/od_neon.png
```

## What else

- Workspace manager that makes it easy to see the status of occupied spaces.
- Real-time monitoring of processor, temp, RAM and disk usage.
- Application launcher dock which can be used for favorite applications.
- Display of pending updates with the possibility to update in one click.
- Quick access to volume and screen brightness controls.
- Display of the local weather in terminal mode.
- Power menu, network devices, sleep control and much more to come.
- Easily customizable with simple CSS/SCSS.
- Pick up everything you need, it's free.

## Troubleshooting

Sometimes hot reloading or `eww reload` doesn't work. In that case use :

```bash
pkill -f -9 eww; eww open-many topbar dock
```

