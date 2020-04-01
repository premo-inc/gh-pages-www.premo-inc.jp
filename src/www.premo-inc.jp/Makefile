server:
	hugo server --themesDir ../themes

build:
	rm -fr public
	HUGO_ENV="production" hugo --gc --themesDir ../themes
	rsync -a --delete public/ ../../docs

install:
	npm install
