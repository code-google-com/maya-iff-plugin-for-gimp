
LOCATION = /usr/freeware

CC = cc
INCLUDES = -I$(LOCATION)/include
LIBS = -L$(LOCATION)/lib32
CFLAGS = -O2 -mips3
GIMPLIBS= -Wl,-rpath,$(LOCATION)/lib32 -L$(LOCATION)/lib32 -lgimp -lgtk -lgdk -lglib
all: MayaIFF

.c.o:
	cc $(INCLUDES) $(CFLAGS) -c  -o $@ $<

MayaIFF: MayaIFF.o
	$(CC) -o MayaIFF MayaIFF.o $(LIBS) $(GIMPLIBS) -lXext -lX11  -lc -lm 
