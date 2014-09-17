volman is a FreeBSD specific volume manager.  It acts 
as a translator of devd(8) events, probing storage 
devices for their file system information, and serving 
this over a FIFO based API to which clients can 
subscribe.  In addition to notifying clients of new 
or lost volumes, it will mount and unmount such 
volumes at the command of subscribing clients.

It runs as root and allows any local clients the 
ability to mount and unmount volumes which are 
detected, regardless of any user privileges.  This 
is intended for single user X11 systems needing 
an easy way of accessing USB flash disks on the fly.

Originally created by:  Aragon Gouveia (jmptbl)
Now maintained by: Uffe Jakobsen

WWW: http://forums.freebsd.org/showthread.php?t=27233
