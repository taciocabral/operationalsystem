make kernel.o
make loader.o
make mykernel.bin

Adicionar ao arquivo grub.cfg (/boot/grub/grub.cfg):

menuentry 'Your System' {
        multiboot /boot/mykernel.bin
        boot
}

Reiniciar Sistema
Selecionar seu sistema no GRUB