## rtmpdump-ksv

An easy way to install rtmpdump with KSV's patches.

### Installing

This has been tested on Ubuntu 16.04 and Debian 8.

Run `apt update` and install dependencies:

    apt install git build-essential libssl-dev

Clone this repo:

    git clone https://github.com/chopraaa/rtmpdump-ksv.git

Change into `rtmpdump-ksv`:

    cd rtmpdump-ksv

Apply KSV's patch:

    patch -p0 -i Patch.diff

Run `make`; use any additional parameters needed:

    make

Install:

    make install prefix=/usr

### License

```RTMP Dump v2.4
(C) 2009 Andrej Stepanchuk
(C) 2009-2011 Howard Chu
(C) 2010 2a665470ced7adb7156fcef47f8199a6371c117b8a79e399a2771e0b36384090
(C) 2011 33ae1ce77301f4b4494faaa5f609f3c48b9dcf82
License: GPLv2
librtmp license: LGPLv2.1
http://rtmpdump.mplayerhq.hu/
```
