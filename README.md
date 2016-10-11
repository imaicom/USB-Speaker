# USB-Speaker setting

$ sudo raspi-config<BR>
•(8)Advanced Options<BR>
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




