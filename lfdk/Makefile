CROSS_COMPILE		=
AS					=   $(CROSS_COMPILE)as
AR					=   $(CROSS_COMPILE)ar
CC					=   $(CROSS_COMPILE)gcc
CPP					=   $(CC) -E
LD					=   $(CROSS_COMPILE)ld
NM					=   $(CROSS_COMPILE)nm
OBJCOPY				=   $(CROSS_COMPILE)objcopy
OBJDUMP				=   $(CROSS_COMPILE)objdump
RANLIB				=   $(CROSS_COMPILE)ranlib
READELF				=   $(CROSS_COMPILE)readelf
SIZE				=   $(CROSS_COMPILE)size
STRINGS				=   $(CROSS_COMPILE)strings
STRIP				=   $(CROSS_COMPILE)strip

CFLAGS				=
LDFLAGS				=   -lpanel -lncurses -g3
OBJS				=   lfdk
LIBS				=	libmem.c libpci.c libio.c libcmos.c


all:
	$(CC) $(CFLAGS) -o $(OBJS) $(OBJS).c $(LIBS) $(LDFLAGS)
	#$(STRIP) $(OBJS)

clean:
	rm -f *.o $(OBJS)


