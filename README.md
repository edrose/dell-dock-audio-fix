# Pulseaudio Fix for Dell USB C and Thunderbolt 3 Docks

Arch linux package that installs config files to allow the audio on the docks to function properly. 

Only two files are placed on the system, these can probably be done on other distros however there is no guarantee that the folders are the same.

    91-pulseaudio.rules 	--> /usr/share/udev/rules.d/
    dell-dock-wd15-usb-audio 	--> /usr/lib/pulseaudio/alsa-mixer/profile-sets/

After installation the contents of ~/.config/pulse or ~/.pulse may need to be removed.

As some of the files included are from Pulseaudio [original source](https://github.com/pulseaudio/pulseaudio) this is distributed under a GNU Lesser licence.
