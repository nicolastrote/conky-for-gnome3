# conkyForGnome3
<p>A conky script for a fast and beauty surpervision on your linux under Gnome 3 desktop</p>
<p></p>
# Installation
<p></p>
<p>You need to install 3 paquages :</p>
<h6>$ sudo apt-get install conky-all hddtemp xsensors</h6>
<p></p>
<h6>$ sudo dpkg-reconfigure hddtemp</h6>
<p>Say "Yes" for all requests.</p>
<p></p>
<p>Download the script and move it under ~/.conkyrc:</p>
<h6>$ sudo mv ~/Download/conkyrc.sh  ~/.conkyrc</h6>
<p></p>
<p>For starting automatically conky with linux, you need adding this under "Startup Applications Preferences" GUI:</p>
<h6>bash -c "sleep 20 ; conky -c ~/.conkyrc"</h6>
<p></p>
# Customisation
<p></p>
<p>Don't forget to change in your conkyrc the name of the internet device "wlan0" by yours.</p>
<p>You can find yours with the command line :</p>
<h6>$ sudo ifconfig</h6>
<h6>eth0      Link encap:Ethernet  HWaddr 84:2b:2b:80:88:b8  </h6>
<h6>...</h6>
<h6>lo        Link encap:Local Loopback </h6> 
<h6>...</h6>
<h6>wlan0     Link encap:Ethernet  HWaddr c0:cb:38:26:48:4b  </h6>
<h6>          inet addr:192.168.0.101  Bcast:192.168.0.255  Mask:255.255.255.0</h6>
<p></p>
<p>and take the name with an IP adress (i.e. 192.168.0.101 => wlan0)<p>
