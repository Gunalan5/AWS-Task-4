lsblk   # find new disk, e.g. /dev/xvdf
sudo mkfs -t ext4 /dev/sdf
sudo mkdir /data
sudo mount /dev/sdf /data
echo "/dev/sdf /data ext4 defaults,nofail 0 2" | sudo tee -a /etc/fstab

df -h
