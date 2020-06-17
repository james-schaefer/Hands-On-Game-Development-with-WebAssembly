## WARNING: 
## Each time to end up with a sane EMCC environment, I end up rerunning the
## steps of EMCC install and activation as outlined here: 
## https://emscripten.org/docs/getting_started/downloads.html
##
## cd ~/git/emsdk
## git pull
## emsdk install latest
## emsdk activate latest
## source ./emsdk_env.sh
##
##  https://stackoverflow.com/questions/51403326/how-to-use-webassembly-from-node-js
##
# Build for chapter 1 code.  
.PHONY: env run build

env:
	echo please remember to update emsdk at for each each new session

build: hello_sdl.c env
	emcc hello_sdl.c --emrun --preload-file font -s USE_SDL_TTF=2 -o hello_sdl.html

hello: hello_sdl.c  

run: 
	firefox http://localhost:12345/
	python3 -m http.server 12345
	#emrun --browser firefox hello_sdl.html
	
list_browsers:
	emrun --list_browsers
