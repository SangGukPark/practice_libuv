CC=gcc
LDLIBS=-luv -lpthread
LDFLAGS=-L/usr/local/lib
INCFLAGS=-I/usr/local/include

OBJS=main.o
TARGET=main

all : $(TARGET)

clean:
	rm -rf *.o;
	rm -rf $(TARGET)

$(TARGET): $(OBJS)
	$(CC) -o $@ $(OBJS) $(LDFLAGS) $(LDLIBS)

.c.o:
	$(CC) -c $< -o $@
