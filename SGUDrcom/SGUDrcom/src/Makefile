CC = g++
LIBS = -lpcap -lpthread
CFLAGS = -DOPENWRT -Os -s -std=c++0x

.PHONY: all
all: EasyDrcom

EasyDrom	: md5.o main.p
	$(CC) $(CFLAGS) -o $@ md5.o main.o $(LIBS)

md5.o	: md5.c
	$(CC) $(CFLAGS) -c $<

main.o : main.c
	$(CC) $(CFLAGS) -c $<
	
clean :
	rm -v *.o EasyDrcom
