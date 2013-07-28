title: Sheevaplug notes
date: 2013-07-27
tags: linux sheevaplug arm
----------------------

## I screwed up my uboot and had to restore it, here is what I learned.

### Sheevaplug is a pain in the ass

Remember:

* openocd isn't reliable under OSX
* Linux VM through OSX works
* Openocd listens on port 4444 after starting
* Use the JTag steps via openocd, must have u-boot
* ELF format is different from bin so you can't flash the same one you boot from


### JTag steps
    reset;sheevaplug_init;load_image u-boot.elf;resume 0x00600000

### Flashing valid uboot afterwards

### UBoot steps
    setenv ipaddr 192.168.10.122;setenv serverip 192.168.10.187;tftpboot uboot.bin


This is a very good guide on installing Debian 5.0
http://www.cyrius.com/debian/kirkwood/sheevaplug/unpack/

This guy seems to have an ARMv5 build of Debian 7.0
http://www.who.is.free.fr/wiki/doku.php?id=armv5


### ArchLinux

Currently failed at getting ArchLinux to install with latest uBoot. No strong reason to use Arch over Debian at the moment (but that may change) so I gave up.

#### Why Arch failed...?

* Seems like the init binary in the Arch initrd just runs the Arch installer. Too bad they didn't use a shell script? Don't know what init should do (despite reading debian init) and didn't want to invest even more time