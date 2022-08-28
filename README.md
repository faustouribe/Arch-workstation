# arch-workstation

sudo pacman -S figlet terminus-font ttf-roboto && yay -S google-chrome archey4 

sudo mv extip /usr/bin/extip && sudo chmod +x /usr/bin/extip

echo "extip" >> ~/.config/zsh/.zshrc

mv xresources ~/.config/x11/

mv settings.ini ~/.config/gtk-3.0/

mv xprofile ~/.config/x11/

mv dmenu-config.h ~/.local/src/dmenu/config.h

mv dwm-config.h ~/.local/src/dwm/config.h

mv dwmblocks-config.h ~/.local/src/dwmblocks/config.h

mv sysact ~/.local/bin/sysact

sudo chmod +x ~/.local/bin/sysact

mv sb-doppler /.local/bin/statusbar/sb-doppler

sudo chmod +x /.local/bin/statusbar/sb-doppler

cd ~/.local/src/dmenu/ 

sudo make && sudo make install


cd ~/.local/src/dwm/ 

sudo make && sudo make install


cd ~/.local/src/dwmblocks/ 

sudo make && sudo make install
