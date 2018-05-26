CC   = cc
OBJS = sub1.o sub2.o

a.out: $(OBJS)
	$(CC) -o $@ $(OBJS)

.c.o:
	$(CC) -c $<

sub1.o: header.h
sub2.o: header.h
