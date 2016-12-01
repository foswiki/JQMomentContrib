FOSWIKI_ROOT?=~/foswiki/trunk/core
TARGET=\
  af.js\
  ar-dz.js\
  ar.js\
  ar-ly.js\
  ar-ma.js\
  ar-sa.js\
  ar-tn.js\
  az.js\
  be.js\
  bg.js\
  bg-x.js\
  bn.js\
  bo.js\
  br.js\
  bs.js\
  ca.js\
  cs.js\
  cv.js\
  cy.js\
  da.js\
  de-at.js\
  de.js\
  dv.js\
  el.js\
  en-au.js\
  en-ca.js\
  en-gb.js\
  en-ie.js\
  en-nz.js\
  eo.js\
  es-do.js\
  es.js\
  et.js\
  eu.js\
  fa.js\
  fi.js\
  fo.js\
  fr-ca.js\
  fr-ch.js\
  fr.js\
  fy.js\
  gd.js\
  gl.js\
  he.js\
  hi.js\
  hr.js\
  hu.js\
  hy-am.js\
  id.js\
  is.js\
  it.js\
  ja.js\
  jv.js\
  ka.js\
  kk.js\
  km.js\
  ko.js\
  ky.js\
  lb.js\
  lo.js\
  lt.js\
  lv.js\
  me.js\
  mi.js\
  mk.js\
  ml.js\
  mr.js\
  ms.js\
  ms-my.js\
  my.js\
  nb.js\
  ne.js\
  nl-be.js\
  nl.js\
  nn.js\
  pa-in.js\
  pl.js\
  pt-br.js\
  pt.js\
  ro.js\
  ru.js\
  se.js\
  si.js\
  sk.js\
  sl.js\
  sq.js\
  sr-cyrl.js\
  sr.js\
  ss.js\
  sv.js\
  sw.js\
  ta.js\
  te.js\
  tet.js\
  th.js\
  tlh.js\
  tl-ph.js\
  tr.js\
  tzl.js\
  tzm.js\
  tzm-latn.js\
  uk.js\
  uz.js\
  vi.js\
  yo.js\
  zh-cn.js\
  zh-hk.js\
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
