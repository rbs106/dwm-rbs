# DWM rbs fork
My personal fork of patched DWM 6.2

# Patches
You can find all the patches on Suckless site

- centerwindowname

- vanitygaps (normal 6.2)

- hide-vacant-tags

# Installing
Depecendies: xorg-server, xorg-xinit, unzip (apt-get install unzip ; pacman -S unzip ; emerge -a unzip), ttf-dejavu

git clone https://github.com/rbs106/dwm-rbs/dwm-rbs.zip

unzip dwm-rbs.zip

cd dwm && sudo make clean install

# Configure
First that you need is .xinitrc on your /home dir, so

sudo cp /etc/X11/xinit/xinitrc ~/.xinitrc

*Now you have it ^^

cd & sudo <editor> .xinitrc
*Delete lines after `twm &` and the `twm &` lol
  
And add this at the bottom
  
**exec dwm
  
# Starting XSERVER
Execute this on tty1 ^^
  
*startx 
  
