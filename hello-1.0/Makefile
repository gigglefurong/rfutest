CC = gcc
CFLAGS = -Wall -Wextra -std=c99
prefix = /usr/local

all: hello

hello: hello.c
	$(CC) $(CFLAGS) -o hello hello.c

clean:
	rm -f hello

install: hello
	install -D hello $(DESTDIR)$(prefix)/bin/hello

.PHONY: all install clean
