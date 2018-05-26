CC = g++
CFLAGS = -g -Wall
OBJS = main.o sub.o
DOCS = $(OBJS:%.o=%.txt)
TARGET = main

.PHONY: clean

%.o: %.cpp
	$(CC) $(CFLAGS) -o $@ -c $<

ALL: $(OBJS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

sub.o: sub.h

docs:
	touch $(DOCS)

clean:
	rm -rf $(OBJS) $(TARGET) $(DOCS)
