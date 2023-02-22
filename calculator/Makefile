CC := gcc
CFLAGS := -Wall

# File names
SRC := main.c addition.c subtraction.c multiplication.c division.c
OBJ := $(SRC:.c=.o)
EXECUTABLE := calculator

# Targets
.PHONY: all clean

all: $(EXECUTABLE)

$(EXECUTABLE): $(OBJ)
	$(CC) $(CFLAGS) $^ -o $@

%.o: %.c operations.h
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJ) $(EXECUTABLE)




