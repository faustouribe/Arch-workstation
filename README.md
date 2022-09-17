# Arch-Workstation Install Script

# Raw process


sudo pacman -S figlet terminus-font ttf-roboto && yay -S google-chrome archey4 

sudo cp extip /usr/bin/extip && sudo chmod +x /usr/bin/extip

echo "extip" >> ~/.config/zsh/.zshrc

cp xresources ~/.config/x11/

cp settings.ini ~/.config/gtk-3.0/

cp xprofile ~/.config/x11/

cp dmenu-config.h ~/.local/src/dmenu/config.h

cp dwm-config.h ~/.local/src/dwm/config.h

cp dwmblocks-config.h ~/.local/src/dwmblocks/config.h

cp sysact ~/.local/bin/sysact

sudo chmod +x ~/.local/bin/sysact

cp sb-doppler ~/.local/bin/statusbar/sb-doppler

sudo chmod +x ~/.local/bin/statusbar/sb-doppler

sudo cp 00-keyboard.conf /etc/X11/xorg.conf.d/

cd ~/.local/src/dmenu/ 

sudo make && sudo make install


cd ~/.local/src/dwm/ 

sudo make && sudo make install


cd ~/.local/src/dwmblocks/ 

sudo make && sudo make install
