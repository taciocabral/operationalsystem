make kernel.o
make loader.o
make mykernel.bin

Adicionar ao arquivo grub.cfg (/boot/grub/grub.cfg):
### BEGIN MYKERNEL ###

menuentry 'Your System' {
        multiboot /boot/mykernel.bin
        boot
}

### END MYKERNEL ###

Reiniciar Sistema
Selecionar seu sistema no GRUB