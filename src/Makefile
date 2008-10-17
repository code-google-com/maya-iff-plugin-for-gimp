
LOCATION = /usr/freeware

CC = gcc
INCLUDES = 
LIBS = 
CFLAGS = -O2 -mips3
GIMPLIBS= -lgimp -lgtk -lgdk -lglib
all: MayaIFF

.c.o:
	cc $(INCLUDES) $(CFLAGS) -c  -o $@ $<

MayaIFF: MayaIFF.o
	$(CC) -o MayaIFF MayaIFF.o $(LIBS) $(GIMPLIBS) -lXext -lX11  -lc -lm 
