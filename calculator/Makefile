CC = gcc
CFLAGS = -Wall

SRC = main.c addition.c subtraction.c multiplication.c division.c
OBJ = $(SRC:.c=.o)

all: calculator

calculator: $(OBJ)
	$(CC) $(CFLAGS) $(OBJ) -o calculator

%.o: %.c operations.h
	$(CC) $(CFLAGS) -c $<

clean:
	rm -f $(OBJ) calculator




