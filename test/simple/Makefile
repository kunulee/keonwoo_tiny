ROOT = ../..

include $(ROOT)/Makefile.common

BINS = simple

.PHONY:	all clean

all:	$(BINS)
.SUFFIXES : .c .o
#%.o:	%.c
#	$(CC) $(CPPFLAGS) $(CFLAGS) $(DEFINES) -c -o $@ $<

$(BINS):	%:	%.o $(TMLIB)
	$(CC) -o $@ $< $(LDFLAGS)

clean:
	rm -f $(BINS) *.o
