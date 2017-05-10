#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ(2.69)
AC_INIT(KISSFFT, 1.30, justin.cui@advantest.com)
AM_INIT_AUTOMAKE()
AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_SRCDIR([kiss_fft.c])
#AM_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CXX
AC_PROG_CC

# Checks for libraries.
LT_INIT
AC_PROG_LIBTOOL

# Checks for header files.
AC_FUNC_ALLOCA
AC_CHECK_HEADERS([limits.h stdlib.h string.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL
AC_C_INLINE
AC_C_RESTRICT
AC_TYPE_SIZE_T
AC_CHECK_TYPES([ptrdiff_t])

# Checks for library functions.
AC_FUNC_ERROR_AT_LINE
#AC_FUNC_MALLOC
AC_HEADER_MAJOR
#AC_FUNC_REALLOC
AC_CHECK_FUNCS([memmove memset select strtol])

AC_CHECK_LIB(m,sincos)
LDFLAGS="-lm"
AC_CHECK_FUNCS([atan2 floor sqrt])

AC_OUTPUT(Makefile)
