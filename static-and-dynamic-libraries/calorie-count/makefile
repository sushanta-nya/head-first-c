hfcal.o: hfcal.c ./includes/hfcal.h
	gcc -I./includes -fPIC -c hfcal.c -o hfcal.o
elliptical.o: elliptical.c ./includes/hfcal.h
	gcc -I./includes -c elliptical.c -o elliptical.o
libs/libhfcal.so: hfcal.o
	gcc -shared hfcal.o -o ./libs/libhfcal.so
elliptical: elliptical.o ./libs/libhfcal.so ./includes/hfcal.h
	gcc elliptical.o -L./libs -lhfcal -o elliptical
