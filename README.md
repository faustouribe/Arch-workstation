# Arch-Workstation Install Script

# Raw process


sudo pacman -S figlet terminus-font ttf-roboto && yay -S google-chrome archey4 

sudo cp extip /usr/bin/extip && sudo chmod +x /usr/bin/extip

cp xresources ~/.config/x11/ \
(change line "*.font: monospace:size=11"
and remove comment signs from solarized)

cp settings.ini ~/.config/gtk-3.0/ \
(change line: "gtk-font-name=Roboto 10")

cp xprofile ~/.config/x11/ \
(change dpi, remove comment in xrdb line)

cp dmenu-config.h ~/.local/src/dmenu/config.h \
(change "monospace:size=12", "NotoColorEmoji:pixelsize=20:antialias=true:autohint=true"

cp dwm-config.h ~/.local/src/dwm/config.h \
( change: "define BROWSER "google-chrome" " "static int swallowfloating = 1;", "static int smartgaps = 1;", "static char *fonts[]          = { "monospace:size=10", "NotoColorEmoji:pixelsize=10:antialias=true:autohint=true"  };" )

cp dwmblocks-config.h ~/.local/src/dwmblocks/config.h \
( comment everything execept "sb-price btc bitcoin, sb-memory, sb-doppler, sb-forecast, sb-volume, sb-battery, sb-clock, sb-internet, sb-help-icon" change static char *delim = " | "; )
 
cp sysact ~/.local/bin/sysact \
(select smaller set of options)

sudo chmod +x ~/.local/bin/sysact

nvim ~/.local/bin/statusbar/sb-doppler
(select a doppler station)

sudo chmod +x ~/.local/bin/statusbar/sb-doppler

sudo cp 00-keyboard.conf /etc/X11/xorg.conf.d/

cd ~/.local/src/dmenu/ 
sudo make && sudo make install

cd ~/.local/src/dwm/ 
sudo make && sudo make install

cd ~/.local/src/dwmblocks/ 
sudo make && sudo make install
