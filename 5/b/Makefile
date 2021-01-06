foobar : foo.o bar.o
	ld -o foobar -s -m elf_i386 foo.o bar.o

foo.o : foo.asm
	nasm -f elf foo.asm

bar.o : bar.c
	gcc -c -m32 bar.c

clean :
	rm foo.o bar.o
