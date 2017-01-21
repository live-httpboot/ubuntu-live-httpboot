ubuntu-live-httpboot
====================

Boot Ubuntu Live media via HTTP.

This uses [httpfs](http://httpfs.sourceforge.net/); therefore the image
is not downloaded completely at the beginning, but parts are loaded
incrementally as they are needed.

The script is designed to run on the live medium itself; see the Releases
section for precompiled kernel/initramfs images for different Ubuntu versions.


How to use
----------

Similar to NFS netboot, pass the kernel parameters `netboot=http nfsroot=http://name.of.your.server/path/to/ubuntu.iso`; make sure to use
the kernel and initrd from this project that matches your Ubuntu version.