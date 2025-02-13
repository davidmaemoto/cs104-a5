CC = gcc
CFLAGS = -Wall -Werror -std=c99

OBJS = main.o addition.o division.o multiplication.o subtraction.o

all: calculator

calculator: $(OBJS)
	$(CC) $(CFLAGS) -o calculator $(OBJS)

main.o: main.c operations.h
	$(CC) $(CFLAGS) -c main.c

addition.o: addition.c operations.h
	$(CC) $(CFLAGS) -c addition.c

division.o: division.c operations.h
	$(CC) $(CFLAGS) -c division.c

multiplication.o: multiplication.c operations.h
	$(CC) $(CFLAGS) -c multiplication.c

subtraction.o: subtraction.c operations.h
	$(CC) $(CFLAGS) -c subtraction.c

clean:
	rm -f *.o calculator
	$(MAKE) all

.PHONY: all clean