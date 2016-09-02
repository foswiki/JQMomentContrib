FOSWIKI_ROOT?=~/foswiki/core
TARGET=moment.js
SUBDIRS=lang
GIT_SOURCES=moment.uncompressed.js

-include $(FOSWIKI_ROOT)/pub/System/JQueryPlugin/Makefile.include

.PHONY: git

git:
	git clone https://github.com/moment/moment.git git

ifneq (,$(wildcard git))
%.uncompressed.js: git/%.js
	cp $< $@
endif

clean: 
	rm -f $(TARGET) *.gz
