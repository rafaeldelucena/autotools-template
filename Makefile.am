## Place generated object files (.o) into the same directory as their source
## files, in order to avoid collisions when non-recursive make is used.
AUTOMAKE_OPTIONS = subdir-objects

ACLOCAL_AMFLAGS = ${ACLOCAL_FLAGS}

bin_PROGRAMS = autotools-template
autotools_template_SOURCES = src/main.c

lib_LTLIBRARIES = libautotools-template-1.0.la
libautotools_template_1_0_ladir = $(includedir)/autotools-template-1.0
libautotools_template_1_0_la_SOURCES = src/libautotools-template.c
libautotools_template_1_0_la_HEADERS = libautotools-template.h
