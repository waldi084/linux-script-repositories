# How to install GNS3 on Arch Based Linux</br>

pacman -S --needed git base-devel

**Install the following packages:**</br>
yay -S gns3-server gns3-gui dynamips ubridge qemu docker wireshark-qt vpcs libvirt gperftools tigervnc

**Add your username to the following groups:**</br>
sudo usermod -aG docker,wireshark,kvm,libvirt username</br>

**Enable systemd services:**</br>
sudo systemctl enable --now docker</br>
sudo systemctl enable --now libvirtd</br>
sudo virsh net-autostart default</br>
