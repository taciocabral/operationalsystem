make kernel.o<br />
make loader.o<br />
make mykernel.bin<br />
make install<br /><br />

### Adicionar ao arquivo grub.cfg (/boot/grub/grub.cfg): ###
menuentry 'Your System' {<br />
        &nbsp;&nbsp;&nbsp;&nbsp;multiboot /boot/mykernel.bin<br />
        &nbsp;&nbsp;&nbsp;&nbsp;boot<br />
}<br /><br />

### Reiniciar Sistema ###
Selecionar seu sistema no GRUB
![alt text](https://i.imgur.com/XKFdLBW.png)
<br />
![alt text](https://i.imgur.com/aUQbhRU.png)


