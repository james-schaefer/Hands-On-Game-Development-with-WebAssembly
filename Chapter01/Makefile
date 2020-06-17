# Build for chapter 1 code.  
.PHONY: env run

env:
	./setup_env.sh

build: hello.c
	emcc hello.c --emrun -o hello.html

run:
	firefox http://localhost:12345
	python3 -m http.server 12345  
	
list_browsers:
	emrun --list_browsers
