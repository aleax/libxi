dnl $XdotOrg: $
dnl
dnl Process this file with autoconf to create configure.

AC_PREREQ([2.57])

AC_INIT(libXi, 1.0, [xorg@lists.freedesktop.org], libXi)
AM_INIT_AUTOMAKE([dist-bzip2])
AM_MAINTAINER_MODE

AM_CONFIG_HEADER(src/config.h)

# Check for progs
AC_PROG_CC
AC_PROG_LIBTOOL

# Checks for pkg-config packages
PKG_CHECK_MODULES(XI, xproto x11 xextproto xext inputproto)
AC_SUBST(XI_CFLAGS)
AC_SUBST(XI_LIBS)

AC_OUTPUT([Makefile
	   src/Makefile
	   man/Makefile
           xi.pc])
