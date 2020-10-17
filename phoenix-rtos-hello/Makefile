TARGET=ia32-generic

include ../phoenix-rtos-build/Makefile.ia32
include ../phoenix-rtos-build/Makefile.common

hello: hello.o
	$(LINK)

all: hello

clean: 
	rm -f *.o hello
