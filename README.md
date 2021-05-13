# ffkbu
FF Hood Bonn with Batman15 and 802.11s


This is the stable site for Gluon 2020.2.3 with wireguard.

__Please remember:
You could use Wireguard only for devices with more than 4Mb of Flash! That means, that f.e. the 841er can only connect to the mesh with fastd!__


## Build Instructions

1. Go in your build system with the user you want to build
2. Download Gluon 2020.2.3. You'll find the informations you'll need under the URL https://gluon.readthedocs.io/en/v2020.2.3/user/getting_started.html
3. Create a directory *site* in your firmware-directory.
4. Download this branch in this directory.
5. Now run *make update*
6. Everything should be complete now. You can start the compiling with the command *make GLUON_TARGET=ar71xx-generic*
7. If everything works you should find your files now in the directory *./output/images/*
