The purpose of these files is to fix the sound on Chromebooks running Ubuntu.

Following full installation of Ubuntu on Intel based Chromebooks running SeaBios an error may occur which results in the lack of sound.

To use the provided script to fix the error do the following steps:

1.) Download the Chromebook-Sound-Fix script
	
2.) Open Terminal and enter or paste the following:
	
	bash ~/Downloads/Chromebook-Sound-Fix


To fix manually complete the following steps:

1.) In the terminal window run the following command:
	
	sudo alsa force-unload

2.)Download the asound.state file and replace the current asound.state file in the following directory:

	/var/lib/alsa/asound.state

3.)Download the analog-output-headphones.conf and repalce the current analog-output-headphones.conf file in the following directory:

	/usr/share/pulseaudio/alsa-mixer/paths/analog-output-headphones.conf

This fix has only been tested on the Acer CB3-111 Chromebook by the author.
# Chromebook-Sound-Fix
