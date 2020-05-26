# Build for chapter 1 code.  
.PHONY: setup_env run

setup_env:
	./setup_env.sh

build: hello.c
	emcc hello.c --emrun -o hello.html

run:
	emrun --browser firefox hello.html
	
list_browsers:
	emrun --list_browsers
