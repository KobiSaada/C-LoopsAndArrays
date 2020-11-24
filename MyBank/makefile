CC = gcc
AR = ar 
CFLAGS = -Wall


all: myBanks MYBANK

myBanks:libmyBank.a
 
main.o:main.c myBank.h
	$(CC) $(CFLAGS) -c main.c
	
MYBANK:main.o libmyBank.a
	$(CC) $(CFLAGS) -o MYBANK main.o libmyBank.a
	
libmyBank.a:myBank.o myBank.h
	$(AR) -rcs libmyBank.a myBank.o myBank.h		

myBank.o: myBank.c myBank.h
	$(CC) $(CFLAGS) -c myBank.c	

.PHONY: clean all 

clean:
	rm *.o *.a MYBANK
