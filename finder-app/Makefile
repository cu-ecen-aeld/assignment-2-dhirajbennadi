INCLUDE_DIRS = 
LIB_DIRS = 
CFLAGS=-Wall -Werror
#CC=aarch64-none-linux-gnu-gcc
#CC=gcc

# ifeq ($(TARGET),CROSS_COMPILE)
#         CC = aarch64-none-linux-gnu-gcc
# else
#         CC = gcc
# endif

CC=$(CROSS_COMPILE)-gcc


HFILES= 
CFILES= writer.c

SRCS= ${HFILES} ${CFILES}

all:	writer

clean:
	-rm -rf writer writer.o

writer: writer.o
	$(CC) -o $@ $<

writer.o: writer.c
	$(CC) $(CFLAGS) -c $<