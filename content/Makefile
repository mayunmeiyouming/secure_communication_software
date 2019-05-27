all: server.o util.o client.o cJSON.o md5.o
	gcc server.o cJSON.o util.o -lm -o server
	gcc client.o cJSON.o md5.o -lm -o client
	rm -f *.o

server.o: server.c
	gcc -c server.c

client.o: client.c
	gcc -c client.c

util.o: util.c
	gcc -c util.c

cJSON.o: cJSON.c
	gcc -c cJSON.c

md5.o: md5.c
	gcc -c md5.c

clean:
	rm -f server client

