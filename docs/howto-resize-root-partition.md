
During the build process the size of the populated filesystem is calculated and
a rather small disk-image is created to hold the filesystem. For this reason
the filesystem you have after installation from a disk-image does not
correspond to the size of your underlying block device. Fortunately it is
quite easy to grow partition and filesystem to match your block device.

### grow partition

assumption: your sd-card block devices are /dev/mmcblk0* (p1, p2)
(you can check that by inspecting /proc/partitions)

```
$ parted /dev/mmcblk0
GNU Parted 3.2
Using /dev/mmcblk0
Welcome to GNU Parted! Type 'help' to view a list of commands.
(parted) print
Model: SD SL16G (sd/mmc)
Disk /dev/mmcblk0: 15.9GB
Sector size (logical/physical): 512B/512B
Partition Table: msdos
Disk Flags: 

Number  Start   End     Size    Type     File system  Flags
 1      2097kB  23.1MB  21.0MB  primary  fat16        boot, lba
 2      23.1MB  273MB   250MB   primary  ext3

(parted) resizepart 2
End?  [273MB]? 4G

# fill in apropriate output here...
```

### grow filesystem

```
$ resize2fs /dev/mmcblk0p2

# fill in apropriate output here...
```
