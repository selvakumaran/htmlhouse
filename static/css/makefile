ifeq ($(shell which lessc),/usr/local/bin/lessc)
	LESSC=/usr/local/bin/lessc
else
	LESSC=node_modules/.bin/lessc
endif
export LESSC

all :
	$(LESSC) -x app.less house.css

local : all

development : all

production : all

install : 
	./less.install

clean :
	rm -f house.css
