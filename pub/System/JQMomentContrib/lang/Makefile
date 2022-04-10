FOSWIKI_ROOT?=~/foswiki/trunk/core
TARGET=$(shell ls ../git/locale/)

-include $(FOSWIKI_ROOT)/pub/System/JQueryPlugin/Makefile.include

GIT_SOURCES=$(TARGET:.js=.uncompressed.js)

git: $(GIT_SOURCES)
	@echo GIT_SOURCES=$(GIT_SOURCES)

ifneq (,$(wildcard ../git))
%.uncompressed.js: ../git/locale/%.js
	cp $< $@

#	sed -i 's/require([^)]*)/moment/g' $@
endif

clean:
	rm -f $(TARGET) $(GIT_SOURCES) *.gz
