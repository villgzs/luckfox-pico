#### Create a bootable SD card with a larger capacity than the default image (6GB).

**on a debian (linux) system**  

    sudo apt install u-boot-tools  

Szerkeszd meg a .env.txt fájlt a kívánt méretre (pl. rootfs:8G).  
Edit the .env.txt file to the desired size (e.g., rootfs:8G). 

Generáld újra az env.img-et:  
Regenerate the env.img:

    mkenvimage -s 32768 -o env.img.new .env.txt
