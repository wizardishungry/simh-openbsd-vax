Notes for getting OpenBSD/vax installed on SIMH
========================
Install SIMH 4.X
```
rake
Follow directions to run simh http://www.openbsd.org/vax-simh.html
```
boot dua2:
````
later
boot dua0:

packages
==========
```
export PKG_PATH=http://mirrors.nycbug.org/pub/OpenBSD/$(uname -r)/packages/$(machine -a)/ 
```
