Notes for getting OpenBSD/vax installed on SIMH
========================
Directions to run simh http://www.openbsd.org/vax-simh.html
My steps:
- Install SIMH 4.X - I have a homebrew tap for mac users. https://github.com/WIZARDISHUNGRY/homebrew-simh
- Download the floppy boot image; the rakefile does this for now
```
rake
```
- Run `./openbsd.simh`
- Wait till you get to the firmware boot prompt
```
boot dua2:
````
- Install OpenBSD
- After rebooting, you can boot the hard disk from the firmware:
```
boot dua0:
```

Misc notes for self
==========
packages:
```
export PKG_PATH=http://mirrors.nycbug.org/pub/OpenBSD/$(uname -r)/packages/$(machine -a)/ 
```
