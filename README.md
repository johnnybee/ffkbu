# ffkbu
FF Hood Bonn mit Batman15 und 802.11s

__This branch is for development only!__
__Please use the branch according to the gluon version for productive systems!!__


Please rename site.conf.wireguard or site.conf.fastd to site.conf according what you want to use and change the package list in site.mk

Please remember:
You could use Wireguard only for devices with __more__ than 4Mb of Flash! That means, that f.e. the 841er can only connect to the mesh with fastd!


## Build Instructions

1. Go in your build system with the user you want to build
2. Download Gluon 2018.1.1. You'll find the informations you'll need under the URL https://gluon.readthedocs.io/en/v2018.1.x/user/getting_started.html
3. Create a directory *site* in your firmware-directory.
4. Download this git in the directory *site*
5. Rename *site.conf.fastd* or *site.conf.wireguard* to *site.conf*
6. Take a look in site.mk and add the packages you need to *GLUON_SITE_PACKAGES*. __There must be no empty line between the package names!__
7. Now run *make update*
8. Everything should be complete now. You can start the compiling with the command *make GLUON_TARGET=ar71xx-tiny* or *make GLUON_TARGET=ar71xx-generic*
9. If everything works you should find your files now in the directory *./output/images/*
