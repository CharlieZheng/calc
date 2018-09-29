default:
	gcc -fPIC -c add.c && \
	gcc -shared -Wl -o libmycalc.so.1.10 add.o && \
	ln -s libmycalc.so.1.10 libmycalc.so && \
	gcc main.c libmycalc.so -o app && \
	./app
clean:
	rm app
	rm *.o
	rm *.so
	rm libmycalc.so.1.10
