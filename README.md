# Conky Theme For Gnome3
A conky script for a fast and beauty surpervision on your linux under Gnome 3 desktop
![alt text](https://github.com/nicolastrote/conkyForGnome3/blob/master/conkyForGnome3.png)

## Installation
You need to install 3 paquages :
```
$ sudo apt-get install conky-all hddtemp xsensors
$ sudo dpkg-reconfigure hddtemp
``` 
 * Say "Yes" for all requests.
 * Download the script and move it under ~/.conkyrc:
```
$ sudo mv ~/Download/conkyrc.sh  ~/.conkyrc
```
 * For starting automatically conky with linux, you need adding this under "Startup Applications Preferences" GUI:
```
bash -c "sleep 20 ; conky -c ~/.conkyrc"
```

## Customisation
Don't forget to change in your conkyrc the name of the internet device "wlan0" by yours.
You can find yours with the command line :
```$ sudo ifconfig```
```
eth0      Link encap:Ethernet  HWaddr 84:2b:2b:80:88:b8
...
lo        Link encap:Local Loopback
...
wlan0     Link encap:Ethernet  HWaddr c0:cb:38:26:48:4b
          inet addr:192.168.0.101  Bcast:192.168.0.255  Mask:255.255.255.0
```
and take the name with an IP adress (i.e. 192.168.0.101 => wlan0)

 * You can make semi-black window disappear with parameter at line 23
```own_window_transparent yes```
 * You can change the transparency of window with parameter at line 22 :
```own_window_argb_value 180```
