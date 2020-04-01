server:
	hugo server --themesDir ../themes

build:
	rm -fr public
	HUGO_ENV="production" hugo --gc --themesDir ../themes
	rsync -a --delete --exclude CNAME --exclude .nojekyll public/ ../../docs

install:
	npm install
