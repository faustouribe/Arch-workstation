# Arch-Workstation Install Script

# Raw process


sudo pacman -S figlet terminus-font ttf-roboto && yay -S google-chrome archey4 

sudo cp extip /usr/bin/extip && sudo chmod +x /usr/bin/extip

cp xresources ~/.config/x11/ \
(change line "*.font: monospace:size=10" for *.font: monospace:size=14"
and remove comment signs from solarized)

cp settings.ini ~/.config/gtk-3.0/ \
(change line: "gtk-font-name=Sans 10" for "gtk-font-name=Roboto 13")

cp xprofile ~/.config/x11/ \
(change dpi, remove comment in xrdb line)

cp dmenu-config.h ~/.local/src/dmenu/config.h \
(change "monospace:size=16", "NotoColorEmoji:pixelsize=8:antialias=true:autohint=true"


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
