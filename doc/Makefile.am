
PANDOC = @PANDOC@

EXTRA_DIST = \
 vep-extras.7.md \
 vep-filter-impact.1.md \
 vepretty.1.md

if HAVE_PANDOC
man_MANS = \
 vep-extras.7 \
 vepretty.1 \
 vep-filter-impact.1
endif

%.7: %.7.md
	$(PANDOC) -s --from=markdown --to=man $< > $@

%.1: %.1.md
	$(PANDOC) -s --from=markdown --to=man $< > $@

clean-local:
	$(RM) $(man_MANS)
