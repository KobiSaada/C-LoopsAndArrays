
all: myBank.o main.o
	gcc -Wall -o all main.o myBank.o

main.o: main.c myBank.h
	gcc -Wall -c main.c

myBank.o: myBank.c myBank.h
	gcc -Wall -c myBank.c	

.PHONY: clean all 

clean:
	rm -f *.o all