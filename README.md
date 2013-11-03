oagd-lauch
==========


### What is this? ###
Oagd-launch is a launcher for the great multiplatform Amiga emulator [fs-uae](http://fs-uae.net).
It can quickly fire up your floppy-based games from your file-manager or the terminal.
It uses built-in configs from fs-uae extended by the ones stored in the [Open Amiga Game Database](http://oagd.net), so no additional configuration should be necessary.
Of course you can still write your favourite default [settings](http://fs-uae.net/options) to $BASEDIR/Configurations/Host.fs-uae


### Requirements ###
- [Linux](http://www.whylinuxisbetter.net)
- [fs-uae](http://fs-uae.net)
- local [Game Database](http://oagd.net) fetched by [fs-uae-launcher](http://fs-uae.net/launcher) (=>2.3.8dev)
- Python 3



### Installation ###
```
cd /usr/local/bin
sudo wget -N https://raw.github.com/sonnenscheinchen/oagd-launch/master/oagd-launch
sudo chmod +x oagd-launch
```


### Usage ###
- From the terminal (recommended):
```
oagd-launch <disk-image>
```

- Using you favourite file manager:
  - open a directory containing your floppy-images
  - right-click on an image, choose "open with..." (or something similar)
  - point to oagd-launch
  - play the game :-)


### Bugs/Limitations ###
- because the launcher needs to checksum all your floppy-images to find the corresponding disks, the first start can be quite slow
- only basic configuration is done for now, it is not as accurate as the "official" fs-uae-launcher yet, but it works for most games...
- save states are disabled, because the configuration is created temporary

