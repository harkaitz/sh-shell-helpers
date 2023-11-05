PROJECT=sh-shell-helpers
VERSION=1.0.0
PREFIX=/usr/local
all:
clean:
install:

## -- BLOCK:license --
install: install-license
install-license: 
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
	cp LICENSE  $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/ls-h-color       $(DESTDIR)$(PREFIX)/bin
	cp bin/crontab-h-exec   $(DESTDIR)$(PREFIX)/bin
	cp bin/find-h-replace   $(DESTDIR)$(PREFIX)/bin
	cp bin/ls-h-category    $(DESTDIR)$(PREFIX)/bin
	cp bin/find-h-close-in-time $(DESTDIR)$(PREFIX)/bin
	cp bin/diff-run         $(DESTDIR)$(PREFIX)/bin
	cp bin/sed-h-recurse    $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
