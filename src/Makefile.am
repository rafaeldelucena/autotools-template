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

libautotools_template_la_includedir = $(includedir)/autotools_template

lib_LTLIBRARIES = libautotools_template.la

libautotools_template_la_SOURCES = \
	autotools_template.c

libautotools_template_la_LDFLAGS = 
 
libautotools_template_la_LIBADD= $(DEPENDENCIES_LIBS)

libautotools_template_la_include_HEADERS = \
	autotools_template.h

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = autotools_template.pc

EXTRA_DIST = \
	autotools_template.pc.in

if ENABLE_TESTS
AM_CFLAGS +=\
	-fprofile-arcs\
	-ftest-coverage

libautotools_template_la_LIBADD += -lgcov
endif
