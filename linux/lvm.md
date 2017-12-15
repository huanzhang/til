pvcreate /dev/vdb
vgcreate vgdata /dev/vdb
lvcreate -L 80G vgdata -n lvdata
mkfs.xfs /dev/mapper/vgdata-lvdata
