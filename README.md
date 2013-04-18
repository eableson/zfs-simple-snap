zfs-simple-snap
===============

A really basic simple snapshot shell script to create ZFS snapshots with a timestamp

Takes none or one argument.

	simple-snap.ksh 

results in snapshots of all available zfs filesystems other than boot zfs filesystems (rpool & syspool)

	simple-snap.ksh <pool>/<filesystem>

will snaphot the filesystem (and children

## Snapshot Naming ##

Snapshots are named with the date in the following format:
"+%Y-%m-%d_%H-%M-%S"" which translates to "2013-04-08_07-11-19"

