test_code: test_code.c encrypt.o checksum.o libhfsecurity.a
	gcc test_code.c -o test_code -lhfsecurity -L. -I.

encrypt.o: encrypt.c encrypt.h
	gcc -c encrypt.c -o encrypt.o

checksum.o: checksum.c checksum.h
	gcc -c checksum.c -o checksum.o

