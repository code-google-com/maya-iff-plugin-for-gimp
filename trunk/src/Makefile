CC = gcc
CFLAGS = -O2
SOURCES = MayaIFF.c
TARGETS = MayaIFF

all: MayaIFF

MayaIFF: $(SOURCES)
	$(CC) $(CFLAGS) -o $@ $< `gimptool-2.0 --cflags` `gimptool-2.0 --libs`

TAGS: $(SOURCES)
	etags $(SOURCES)

clean:
	@rm -fr *.o *~ $(TARGETS) TAGS
