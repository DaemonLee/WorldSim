# Makefile for people library unit tests

all: clean utest

clean:
	rm -f *.o utest

utest: ../people.h ../libpeople.a utest.c
	$(CC) $(CFLAGS) -lm -o utest utest.c ../libpeople.a $(LIB)/libgender.a $(LIB)/libcal.a $(LIB)/libwstime.a $(LIB)/librng.a

runtest: utest
	./utest

ROOT = ../..
include $(ROOT)/Makefile.inc
