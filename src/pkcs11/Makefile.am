MAINTAINERCLEANFILES = $(srcdir)/Makefile.in

AM_CPPFLAGS = -I$(top_srcdir)/src

lib_LTLIBRARIES = libsc-hsm-pkcs11.la

libsc_hsm_pkcs11_la_SOURCES = dataobject.c debug.c object.c p11generic.c p11mechanisms.c p11objects.c \
			p11session.c p11slots.c secretkeyobject.c session.c slot.c slotpool.c strbpcpy.c \
			token.c
libsc_hsm_pkcs11_la_LDFLAGS = $(AM_LDFLAGS) \
	-export-symbols "$(srcdir)/libpkcs11.exports" \
	-module -shared -avoid-version -no-undefined