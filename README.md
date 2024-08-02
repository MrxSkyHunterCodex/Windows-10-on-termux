# Windows-10-on-termux
Full size 1,4 gb





apt update && apt upgrade -y
pkg install x11-repo
2) Now we need to give the storage access to termux for this type “termux-setup-storage” and press enter.

termux-setup-storage
3) Now install the required Qemu package for this type “pkg install qemu-system-x86-64-headless

pkg install qemu-system-x86-64-headless -y






qemu-system-x86_64 \
Choose Windows 10 file location (copy and paste the path of your downloaded and extracted qemu windows10 image file)

-hda /storage/emulated/0/Download/Windows-10.qcow2 \
Select Max CPU Core for Windows 10 machine




cpu max \
-smp cpus=4,cores=4,threads=1,sockets=1 \
Choose Ram your Windows 10 machine (Provide ram ranging from 400-3047M)

-m 2030M \
-machine pc \
Select Screen Size for Windows 10 VNC

-vga vmware -full-screen \
-overcommit mem-lock=off \
-accel tcg,thread=single \
-rtc base=localtime \
-net user -net nic,model=rtl8139 \
 

Access Mobile Files on Windows 10 Some Folder (copy and paste the path of the Disk folder)

-drive file=fat:rw:/storage/emulated/0/Download/Disk \
Start VNC Server

-vnc 127.0.0.1:1





download for now :)
https://drive.google.com/file/d/0B9zhkeeW3VdVRk1qUjZFUHh0Wm8/view?usp=drivesdk
