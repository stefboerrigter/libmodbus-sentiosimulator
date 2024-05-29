EXTRA_DIST = README.md LICENSE

noinst_PROGRAMS = \
	sentio-sim-server

common_ldflags = \
	$(top_builddir)/src/libmodbus.la

sentio_sim_server_SOURCES = sentio-sim-server.c
sentio_sim_server_LDADD = $(common_ldflags)


AM_CPPFLAGS = \
    -include $(top_builddir)/config.h \
    -DSYSCONFDIR=\""$(sysconfdir)"\" \
    -DLIBEXECDIR=\""$(libexecdir)"\" \
    -I${top_srcdir}/src \
    -I${top_builddir}/src

AM_CFLAGS = ${my_CFLAGS}

CLEANFILES = *~ *.log
