
#make fname=helloworld
fname=test

default: clean test

test: link
	./$(fname).ex

link: assemble
	gcc -m32 -nostdlib -nostdinc -o $(fname).ex $(fname).o

assemble:
	nasm -f elf $(fname).asm


clean:
	rm -rf *.o *.ex


