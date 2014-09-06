LVM-Snapshot-Rotate
===================

Allows you to create periodic LVM Snapshots, rotate them and delete them when they exceed the set time.

I developed this script for the automatic creation of LVM Snapshots and for automatically remove them after a set time.
The script at the moment does the following:

1. Creates a LVM Snapshot of a set volume and names with a timestamp
2. Mounts the snapshot under /opt/snapshots/snapname
3. Each time it's run checks if existing snapshots are beyond the set expiration time and removes them.

Future features planned:
* Support for COW offloading
* Better custom parameters support
