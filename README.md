##### I'll be honest, I meant to upload this ages ago, but completely forgot. I can't remember which files were specifically needed, but I have added in my Wireplumber config. If someone wants to declutter this then go for it - the audio setup works for me, so until it inevitably breaks again I'm not going to spend too much time on this to protect my sanity. 


# steelseries-gamedac-pipewire
Enable ChatMix and surround sound on the Steelseries Arctis Pro using Pipewire profile files and Wireplumber configs. Based off [the work by Witek094](https://github.com/Witek094/steelseries-arctis-pro-wireless-pulseaudio-profile)
## Installation
Copy 91-pulseaudio-steelseries-gamedac.rules to /etc/udev/rules.d 

Copy steelseries-gamedac-usb-audio.conf to /usr/share/pulseaudio/alsa-mixer/profile-sets 

Copy steelseries-gamedac-input.conf, steelseries-gamedac-output-chat.conf, steelseries-gamedac-output-game.conf to /usr/share/pulseaudio/alsa-mixer/paths/ 

Copy 51-steelseries-gamedac.conf to ~/.config/wireplumber/wireplumber.conf.d



**WARNING**: At the moment, you can't use the DAC's "Hi-Res" mode while these profiles are installed (this will be updated when I find a way). To restore original functionality, just delete the files you copied again and replug the DAC
