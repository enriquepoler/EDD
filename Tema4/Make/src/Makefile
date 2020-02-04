CC=gcc
CFLAGS=-Wall -g
calcula: calcula.c calc.o
	$(CC) $(CFLAGS) calcula.c calc.o calcula
calc.o: calc.c calc.h
	$(CC) $(CFLAGS) -c calc.c calc.o
.PHONY: clean
clean: 
	rm -rf *.o
	rm calcula