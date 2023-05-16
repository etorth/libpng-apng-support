CC = gcc
CFLAGS = -std=c99 -Wall -pedantic -O2
LIBS = -lz -lpng

all: png apng

png: load1png load2png load5apng load6apng load7png save1png

apng: load3apng load4apng load8apng resave2gray resave2rgba save2apng

load1png: load1png.c
	$(CC) $(CFLAGS) -o load1png load1png.c $(LIBS) 

load2png: load2png.c
	$(CC) $(CFLAGS) -o load2png load2png.c $(LIBS) 

load3apng: load3apng.c
	$(CC) $(CFLAGS) -o load3apng load3apng.c $(LIBS) 

load4apng: load4apng.c
	$(CC) $(CFLAGS) -o load4apng load4apng.c $(LIBS) 

load5apng: load5apng.c
	$(CC) $(CFLAGS) -o load5apng load5apng.c $(LIBS) 

load6apng: load6apng.c
	$(CC) $(CFLAGS) -o load6apng load6apng.c $(LIBS) 

load7png: load7png.c
	$(CC) $(CFLAGS) -o load7png load7png.c $(LIBS) 

load8apng: load8apng.c
	$(CC) $(CFLAGS) -o load8apng load8apng.c $(LIBS) 

resave2gray: resave2gray.c
	$(CC) $(CFLAGS) -o resave2gray resave2gray.c $(LIBS) 

resave2rgba: resave2rgba.c
	$(CC) $(CFLAGS) -o resave2rgba resave2rgba.c $(LIBS) 

save1png: save1png.c
	$(CC) $(CFLAGS) -o save1png save1png.c $(LIBS) 

save2apng: save2apng.c
	$(CC) $(CFLAGS) -o save2apng save2apng.c $(LIBS) 

clean: 
	rm -f load1png
	rm -f load2png
	rm -f load3apng
	rm -f load4apng
	rm -f load5apng
	rm -f load6apng
	rm -f load7png
	rm -f load8apng
	rm -f resave2gray
	rm -f resave2rgba
	rm -f save1png
	rm -f save2apng

test: 
	./load1png clock4.png
	./load2png clock4.png
	./load3apng clock4.png
	./load4apng clock4.png
	./load5apng clock4.png
	./load6apng clock4.png
	./load7png clock4.png
	./load8apng clock4.png
	./resave2gray clock4.png
	./resave2rgba clock4.png
	./save1png
	./save2apng
