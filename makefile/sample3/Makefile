program = hello
objs = hello.o edajima.o
CC = gcc
CFLAGS = -g -Wall

.SUFFIXES: .c .o

$(program): $(objs)
	$(CC) -o $(program) $^

.c.o:
	$(CC) $(CFLAGS) -c $<

.PHONY: clean
clean:
	$(RM) $(program) $(objs)
