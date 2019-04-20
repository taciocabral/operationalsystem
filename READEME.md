make kernel.o<br />
make loader.o<br />
make mykernel.bin<br /><br />

Adicionar ao arquivo grub.cfg (/boot/grub/grub.cfg):<br /><br />

menuentry 'Your System' {<br />
        multiboot /boot/mykernel.bin<br />
        boot<br />
}<br /><br />

Reiniciar Sistema<br />
Selecionar seu sistema no GRUB