<h1>Example writing operating system on C and ASM </h1>


## Compile Commands
<ul>
  <li>
    1. nasm -f elf32 sys/boot/boot.asm -o build/boot.o
    2. gcc -m32 -c sys/kernel/header.c -o build/krnl.o
    3. ld -m elf_i386 -T link.ld -o kernel build/boot.o build/krnl.o
  </li>
</ul>
