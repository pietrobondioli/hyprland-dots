# My .Files

## Description


## Instructions

### Install Archlinux w/ Hyprland

### Install yay

```
pacman -S --needed git base-devel
```

```
git clone https://aur.archlinux.org/yay.git
```

```
cd yay && makepkg
```

### Clone this repo and copy initial hypr config

```
git clone https://github.com/pietrobondioli/my-dots.git
```

```
cp -r ./my-dots/hypr/* ~/.config/hypr/
```


### Configure zsh and oh-my-zsh

Copy kitty config from this repo:
```
cp -r ./my-dots/kitty/* ~/.config/kitty/
```

Install zsh:

```
yay -S zsh
```

Install oh-my-zsh:
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Copy theme from this repo:
```
cp ./oh-my-zsh/xxf.zsh-theme ~/.oh-my-zsh/custom/themes/
```

Clone plugins:
```
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions & git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
```

Fix permissions for syntax plugin:
```
chmod 700 ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
```

Get .zshrc from this repo:
```
cp ./oh-my-zsh/.zshrc ~/
```

Install neofetch
```
yay -S neofetch
```

Copy neofetch config from this repo:
```
cp -r ./my-dots/neofetch/* ~/.config/neofetch
```

If on zsh installating it didn't made zsh the default shell do it manually:
```
chsh -s $(which zsh)
```

yay -S swaylock-effects rofi dunst xdg-desktop-portal-hyprland-git \
swappy grim slurp wl-clipboard thunar polkit-gnome python-requests \
pavucontrol brightnessctl bluez bluez-utils blueman \
network-manager-applet gvfs thunar-archive-plugin file-roller btop \
pacman-contrib ttf-jetbrains-mono-nerd noto-fonts-emoji \
lxappearance xfce4-settings waybar-hyprland swaybg fcitx5 \
pomotroid hyprpicker wf-recorder python-requests swayidle thunar \
nwg-look-bin

yay -S qt5-wayland qt5ct qt6-wayland qt6ct qt5-svg qt5-quickcontrols2 \
qt5-graphicaleffects gtk3 cliphist \
dracula-gtk-theme dracula-icons-git

yay -S otf-font-awesome ttf-jetbrains-mono-nerd ttf-jetbrains-mono \
otf-font-awesome-4 ttf-droid ttf-fantasque-sans-mono \
adobe-source-code-pro-fonts noto-fonts-emoji

yay -S zathura zathura-pdf-mupdf

yay -S gnome-keyring seahorse

"password-store": "gnome" on vscode command "Preferences: Configure Runtime Arguments"

yay -S visual-studio-code-bin rider

yay -S aspnet-targeting-pack-preview-bin aspnet-runtime-preview-bin \
aspnet-targeting-pack-6.0 aspnet-targeting-pack aspnet-runtime-6.0 \
aspnet-runtime

yay -S dotnet-source-built-artifacts-6.0 dotnet-targeting-pack-6.0 \
dotnet-runtime-6.0 dotnet-sdk-6.0 \
dotnet-targeting-pack-preview-bin dotnet-runtime-preview-bin \
dotnet-sdk-preview-bin dotnet-host-preview-bin \
dotnet-runtime dotnet-host dotnet-sdk dotnet-targeting-pack \
dotnet-source-built-artifacts
