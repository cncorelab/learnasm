sandbox: sandbox.o
	ld -m elf_i386 -o sandbox sandbox.o
sandbox.o: sandbox.asm
	nasm -f elf -g -F stabs sandbox.asm -l sandbox.lst
clean:
	rm *.lst
	rm *.o
	rm sandbox
run: sandbox
	./sandbox
