ACLOCAL_AMFLAGS = -I m4
AM_DISTCHECK_CONFIGURE_FLAGS = --enable-relocatable

SUBDIRS = lib src providers tests

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = enchant.pc

EXTRA_DIST =		\
	enchant.pc.in	\
	README 		\
	HACKING 	\
	NEWS 		\
	ChangeLog 	\
	AUTHORS 	\
	COPYING.LIB	\
	m4/gnulib-cache.m4

ALL_SOURCE_FILES = \
	bootstrap.conf \
	configure.ac \
	Makefile.am \
	src/Makefile.am \
	src/*.[chi] \
	providers/Makefile.am \
	providers/*.[ch] \
	providers/*.cpp \
	providers/*.mm

loc:
	cloc --force-lang="Bourne Shell",conf $(ALL_SOURCE_FILES)
