# arch-workstation

sudo pacman -S figlet terminus-font ttf-roboto && yay -S google-chrome archey4 

sudo mv extip /usr/bin/extip && sudo chmod +x /usr/bin/extip

echo "extip" >> ~/.bashrc

echo "export PATH=/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl:/home/mrfox/.local/bin:/home/mrfox/.local/bin/__pycache__:/home/mrfox/.local/bin/cron:/home/mrfox/.local/bin/statusbar:/home/mrfox/bin/gyb" >> ~./bashrc

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
