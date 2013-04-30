CFLAGS = -I../include -pthread -O1
LIB    = ../lib/x11/libglfw.a
LFLAGS = $(LIB) -lrt -lX11 -lGLU -lGL -pthread -lm -lXrandr

all: ms

ms: ms.o ../lib/x11/libglfw.a
	gcc ms.o $(LFLAGS) -o ms

ms.o: ms.c
	gcc -c $(CFLAGS) ms.c

clean:
	rm -f ms
	rm -f *.o

