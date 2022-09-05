Change  ~/.xprofile
    xrandr --dpi 144

Change ~/.config/gtk-3.0/settings.ini
    gtk-font-name=Roboto 10

# Chrome
    Create vim ~/.config/chrome-flags.conf

add
    --force-device-scale-factor=2
    
Settings/Appearance
    Adjust fonts

# Firefox
Open a new tab and enter the following text in the address bar
    about:config

Enter the following text in the search box
    layout.css.devPixelsPerPx

The value layout.css.devPixelsPerPx will appear in the list. 
By default, its value data is set to -1.0, which means "follow the system settings". 
You can override it by changing the value to a positive number.
Start changing it with 1.5 and continue until you satisfied with what you see.

    me gusto "2"


To change user interface density in Firefox, do the following.

1.- Click the hamburger menu button and click the "Customize" item.
2.- Click on the "Density" item at the bottom of the "Customize" pane.
3.- Click on either Compact,Default or Touch item in the drop down list according to what you want. 
    Compact is the smallest UI type, Touch is the biggest one.
    
    me gustó compact
