# Compiler and flags
# TODO 1
CC = ____

# TODO 2 (hint: add an optimization flag)
CFLAGS = -fopenmp ____

# Targets
TARGET = final

# TODO 3 (hint: list all object files)
OBJS = ____

# TODO 4 (hint: install prefix, e.g. $(HOME)/lab3-1; do not put a comment on the same line)
PREFIX = ____

# Default target
$(TARGET) : $(OBJS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

# Compile each source file into object file
main.o : main.c vector.h matrix.h
	$(CC) $(CFLAGS) -c main.c

vector.o : vector.c vector.h
	$(CC) $(CFLAGS) -c vector.c

# TODO 5 (hint: matrix.c includes a header file)
matrix.o : matrix.c ____
	$(CC) $(CFLAGS) -c ____

# TODO 6 (hint: copy the binary to $(PREFIX)/bin)
# Install target
install : $(TARGET)
	mkdir -p ____
	cp $(TARGET) ____

# Clean up
.PHONY : clean install
clean :
	rm -f $(TARGET) $(OBJS)
