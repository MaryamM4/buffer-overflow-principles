all:	server.c httpd.c parse.c token.c http-tree.c
	gcc -g -o touchstone server.c
	gcc -g -o httpd httpd.c token.c parse.c http-tree.c handle.c

clean:
	rm -rf touchstone httpd