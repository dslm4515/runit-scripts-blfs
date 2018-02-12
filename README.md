# runit-scripts-blfs
A collection of scripts for a Runit init-system for LFS/BLFS. Some of the scripts from https://github.com/inthecloud247/runit-for-lfs did not work for me and required modification. Such changes are saved here.

Runit was developed by Gerrit Pape. His work can be found at http://smarden.org/runit/index.html.

These scripts are for Linux From Scratch system that uses runit as the init. More info at http://www.linuxfromscratch.org.

To use:
(1) Copy the desired folder(s) to /etc/sv.
(2) Link desired folder(s) to /etc/runit/runsvdir/multi

Format:
Each folder is the name of service with a "run" script inside. The run script is executed by runit.

Notes:
+ Could not find a good lightDM script...used a script from Void Linux, but lightDM never loads, unless run by root explicitly. Therefore test system had to use lxdm instead.
