# Edit: this has now been fixed in PulseAudio but I'll keep the repo here for reference. If you are searching for a current Dell Dock Pulseaudio issue then this probably won't fix it. Take a look at [this comment thread](https://github.com/edrose/dell-dock-audio-fix/issues/2) for a link to a current bug fix.

# Pulseaudio Fix for Dell USB C and Thunderbolt 3 Docks

Arch linux package that installs config files to allow the audio on the docks to function properly. 

Only two files are placed on the system, these can probably be done on other distros however there is no guarantee that the folders are the same.

    91-pulseaudio.rules         --> /usr/share/udev/rules.d/


    dell-dock-wd15-usb-audio	--> /usr/lib/pulseaudio/alsa-mixer/profile-sets/

After installation the contents of ~/.config/pulse or ~/.pulse may need to be removed.

As some of the files included are from Pulseaudio ([pulseaudio/pulseaudio@60c0edd](https://github.com/pulseaudio/pulseaudio/commit/60c0edd5286dbb731c671ad3e6886c1e3e1eb067)) this is distributed under a GNU Lesser licence.
