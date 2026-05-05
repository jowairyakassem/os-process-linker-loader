all: process_creation role_of_linker role_of_loader

process_creation: process_creation.c
	gcc process_creation.c -o process_creation

role_of_linker: file1jk.c file2jk.c
	gcc file1jk.c file2jk.c -o role_of_linker

role_of_loader: role_of_loader.c
	gcc role_of_loader.c -o role_of_loader

run_ex1: process_creation
	./process_creation

run_ex5:
	gcc file1jk.c file2jk.c -o role_of_linker
	./role_of_linker

run_ex6: role_of_loader
	./role_of_loader
	ldd ./role_of_loader

clean:
	rm -f process_creation role_of_linker role_of_loader

