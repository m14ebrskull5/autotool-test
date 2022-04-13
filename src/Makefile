all: jupiter
main=main.c
jupiter: main.c foo
		main=main.c; \
		ls; \
		gcc -O0 -o main ${main} -lz -L.

clean:
		-rm jupiter

mytarget=foo
$(mytarget):
	gcc -shared -fPIC -o libz.dll -c $(mytarget).c; \
	# ar -shared libbar.a bar

mytarget=bar

clean: src/bar.o src/bar.a src/libbar.dll src/main.exe
	rm src/bar.o src/bar.a src/libbar.dll src/main.exe