test:main.o circle.o
	gcc main.o circle.o -o test

main.o:main.c
	gcc -c main.c -o main.o

circle.o:circle.c
	gcc -c circle.c -o circle.o

.PHONY:
run:
	make
	chmod 777 test
	./test
