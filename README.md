# USB-Speaker setting

$ sudo raspi-config<BR>
•(9)Advanced Options<BR>
•A9 Audio<BR>
•Audio - Auto<BR>
 <BR>
$ lsusb<BR>
<BR>
$ sudo vi /usr/share/alsa/alsa.conf<BR>
<BR>
comment out<BR>
"~/.asoundrc"  >  # "~/.asoundrc"<BR>
<BR>
Modify the two line<BR>
defaults.ctl.card 0 > defaults.ctl.card 1<BR>
defaults.pcm.card 0 > defaults.pcm.card 1<BR>
<BR>
sudo reboot<BR>
alsamixer<BR>
<BR>
sudo apt-get install mpg123<BR>
  
cd /usr/share/scratch/Media/Sounds/Animal/;aplay *.wav  
cd /usr/share/scratch/Media/Sounds/Animal/;aplay *.mp3  
cd /usr/share/scratch/Media/Sounds/Effects/;aplay *.wav  
cd /usr/share/scratch/Media/Sounds/Electronic/;aplay *.wav  
cd /usr/share/scratch/Media/Sounds/Human/;aplay *.wav  
cd /usr/share/scratch/Media/Sounds/Human/;mpg321 *.mp3  
cd /usr/share/scratch/Media/Sounds/Instruments/;aplay *.wav  
cd /usr/share/scratch/Media/Sounds/"Music Loops"/;mpg321 *.mp3  
cd /usr/share/scratch/Media/Sounds/Percussion/;aplay *.wav  
cd /usr/share/scratch/Media/Sounds/Vocals/;mpg321 *.mp3  
cd /usr/share/scratch/Media/Sounds/Vocals/;aplay *.wav  
cd /usr/share/sounds/alsa/;aplay *.wav  
cd /usr/lib/python3/dist-packages/pygame/examples/data/;aplay *.wav  
cd /usr/lib/python2.7/dist-packages/pygame/examples/data/;aplay *.wav    
