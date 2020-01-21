mdadm --detail /dev/md0

mdadm --manage /dev/md0 --remove /dev/sdb1

Copy partition table!:
sfdisk -d /dev/sda | sfdisk /dev/sdb

mdadm --manage /dev/md0 --add /dev/sdb1
