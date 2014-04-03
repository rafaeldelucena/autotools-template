noinst_PROGRAMS = $(TEST_PROGS)

PRODUCTION_CODE_INCLUDES = -I$(top_builddir)/src
PRODUCTION_CODE_LIBS = $(top_builddir)/src/libautotools_template.la

AM_CPPFLAGS = \
	$(CPPUTEST_CFLAGS)\
	$(PRODUCTION_CODE_INCLUDES)

AM_CFLAGS =	-Werror\
			-Wall\
			-g

AM_CXXFLAGS = $(AM_CFLAGS)

TEST_PROGS = autotools_template_tests

autotools_template_tests_SOURCES = autotools_template_tests.cpp
autotools_template_tests_LDADD = $(CPPUTEST_LIBS)\
						$(PRODUCTION_CODE_LIBS)

check_PROGRAMS = $(TEST_PROGS)

TESTS = $(TEST_PROGS)
