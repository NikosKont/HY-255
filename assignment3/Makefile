all: list hash

GCC = gcc -Wall -ansi -pedantic -g

list:
	$(GCC) -c ./src/symtablelist.c -o ./src/symtablelist.o
	$(GCC) ./src/testsymtab.c ./src/symtablelist.o -o testsymtab.exe

hash:
	$(GCC) -c ./src/symtablehash.c -o ./src/symtablehash.o
	$(GCC) ./src/testsymtab.c ./src/symtablehash.o -o testsymtab.exe

clean:
	-rm -f *.exe ./src/*.o