AM_CPPFLAGS = \
	-DPACKAGE_LOCALE_DIR=\""$(localedir)"\" \
	-DPACKAGE_SRC_DIR=\""$(srcdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(pkgdatadir)"\" \
	$(DEPENDENCIES_CFLAGS)

AM_CFLAGS =\
		   -Wextra
		   -Werror\
		   -Wall\
		   -g

libautotools_template_la_includedir = $(includedir)/autotools-template

lib_LTLIBRARIES = libautotools-template.la

libautotools_template_la_SOURCES = \
	autotools-template.c

libautotools_template_la_LDFLAGS = 
 
libautotools_template_la_LIBADD= $(DEPENDENCIES_LIBS)

libautotools_template_la_include_HEADERS = \
	autotools-template.h

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = autotools-template.pc

EXTRA_DIST = \
	autotools-template.pc.in

if ENABLE_TESTS
AM_CFLAGS +=\
			-fprofile-arcs\
			-ftest-coverage

libautotools_template_la_LIBADD += -lgcov
endif
