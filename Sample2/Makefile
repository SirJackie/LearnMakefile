test:main.o
	gcc main.o -o test

main.o:main.c
	gcc -c main.c -o main.o

.PHONY:
run:
	make
	chmod 777 test
	./test
