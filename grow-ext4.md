
Scan for changes:
echo 1 > /sys/class/block/sda/device/rescan
Increase partition to maximum size
growpart sda 2
resize2fs /dev/sda2

An other option is to delete the partition, create it again and then run resize2fs
