vidbuff1: vidbuff1.o
	ld -m elf_i386 -o vidbuff1 vidbuff1.o
vidbuff1.o: vidbuff1.asm
	nasm -f elf -g -F stabs vidbuff1.asm
clean:
	rm *.lst
	rm *.o
	rm vidbuff1
run: vidbuff1
	./vidbuff1
