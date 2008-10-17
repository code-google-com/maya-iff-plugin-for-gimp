
LOCATION = /usr/freeware

CC = gcc
INCLUDES = 
LIBS = 
CFLAGS = -O2
all: MayaIFF TAGS

.c.o:
	$(CC) $(INCLUDES) $(CFLAGS) -c  -o $@ $<

MayaIFF: MayaIFF.c
	$(CC) $(CFLAGS) -o $@ $< `gimptool-2.0 --cflags` `gimptool-2.0 --libs`


TAGS: MayaIFF.c
	etags MayaIFF.c

clean:
	@rm -fr *.o *~ MayaIFF TAGS
