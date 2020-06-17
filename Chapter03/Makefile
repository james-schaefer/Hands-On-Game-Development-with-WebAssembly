# Build for chapter 1 code.  
.PHONY: env run 

env:
	./setup_env.sh

build: webgl.c webgl_shell.html 
	emcc webgl.c --emrun --shell-file webgl_shell.html -o webgl.html

run: webgl.html 
        firefox http://localhost:12345
        python3 -m http.server 12345  
	
list_browsers:
	emrun --list_browsers
