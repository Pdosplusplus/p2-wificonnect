# Guide to connect to a wifi for terminal

To connect a wifi first Up the wlan0:

```bash
$ sudo ifconfig wlan0 up  
```

list of wifi in the area:

```bash
$ sudo iwlist wlan0 scan
```

Check of ```ESSID``` of the red to want connect

And now connect to wifi:

```bash
$ sudo nmcli d wifi connect "ESSID" password "the-password" iface wlan0
```

A real case:

```bash
$ sudo nmcli d wifi connect "Generico" password "12345678910" iface wlan0
```

