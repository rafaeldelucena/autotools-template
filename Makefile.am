SUBDIRS = src

if ENABLE_TESTS
SUBDIRS += tests
endif

DIST_SUBDIRS = $(SUBDIRS)

autotools_templatedocdir = ${prefix}/doc/autotools-template
autotools_templatedoc_DATA = \
	README\
	COPYING\
	AUTHORS\
	ChangeLog\
	INSTALL\
	NEWS


EXTRA_DIST = $(autotools_templatedoc_DATA)


# Remove doc directory on uninstall
uninstall-local:
	-rm -r $(autotools_templatedocdir)

coverage:
if ENABLE_COVERAGE
	gcovr -x -r .. -e ".+\.test\.cpp" --object-directory=src > coverage.xml
else
	@echo "To generate coverage report, please run ./configure with --enable-coverage"
endif
