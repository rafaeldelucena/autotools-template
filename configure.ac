AC_INIT([AutotoolsExample], [0.1], [rafael@casamarelahacking.com.br])
AC_PREREQ([2.59])
AM_INIT_AUTOMAKE([1.10 no-define])
AC_CONFIG_HEADERS([config.h])
AC_PROG_CC
AC_PROG_CXX

dnl Example of default-disabled feature
AC_ARG_ENABLE([tests], AS_HELP_STRING([--enable-tests], [Enable Unit Tests]))

AM_CONDITIONAL([TESTS_ENABLED], [test "x$enable_bar" = "xyes"])

AC_CONFIG_FILES([Makefile])
AC_OUTPUT
