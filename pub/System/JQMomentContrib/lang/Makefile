FOSWIKI_ROOT?=~/foswiki/trunk/core
TARGET= \
  af.js \
  ar.js \
  ar-ma.js \
  ar-sa.js \
  ar-tn.js \
  az.js \
  be.js \
  bg.js \
  bn.js \
  bo.js \
  br.js \
  bs.js \
  ca.js \
  cs.js \
  cv.js \
  cy.js \
  da.js \
  de-at.js \
  de.js \
  el.js \
  en-au.js \
  en-ca.js \
  en-gb.js \
  eo.js \
  es.js \
  et.js \
  eu.js \
  fa.js \
  fi.js \
  fo.js \
  fr-ca.js \
  fr.js \
  fy.js \
  gl.js \
  he.js \
  hi.js \
  hr.js \
  hu.js \
  hy-am.js \
  id.js \
  is.js \
  it.js \
  ja.js \
  jv.js \
  ka.js \
  km.js \
  ko.js \
  lb.js \
  lt.js \
  lv.js \
  me.js \
  mk.js \
  ml.js \
  mr.js \
  ms.js \
  ms-my.js \
  my.js \
  nb.js \
  ne.js \
  nl.js \
  nn.js \
  pl.js \
  pt-br.js \
  pt.js \
  ro.js \
  ru.js \
  si.js \
  sk.js \
  sl.js \
  sq.js \
  sr-cyrl.js \
  sr.js \
  sv.js \
  ta.js \
  th.js \
  tl-ph.js \
  tr.js \
  tzl.js \
  tzm.js \
  tzm-latn.js \
  uk.js \
  uz.js \
  vi.js \
  zh-cn.js \
  zh-tw.js

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
