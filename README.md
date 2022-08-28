# Arch-workstation

Instalar programas basicos

sudo pacman -S figlet terminus-font ttf-roboto && yay -S google-chrome archey4 

Crear extip

sudo mv extip /usr/bin/extip && sudo chmod +x /usr/bin/extip

sudo mv xresources ~/.config/x11/

sudo mv settings.ini ~/.config/gtk-3.0/

sudo mv xprofile ~./config/x11/

sudo mv dmenu-config.h ~/.local/src/dmenu/

cd ~/.local/src/dmenu/ 

sudo make && sudo make install

sudo mv dwm-config.h ~/.local/src/dwm/

cd ~/.local/src/dwm/ 

sudo make && sudo make install

sudo mv dwmblocks-config.h ~/.local/src/dwmblocks/

cd ~/.local/src/dwmblocks/ 

sudo make && sudo make install

sudo mv sysact ~/.local/bin/


