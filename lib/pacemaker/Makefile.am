#
# Copyright 2004-2018 Andrew Beekhof <andrew@beekhof.net>
#
# This source code is licensed under the GNU General Public License version 2
# or later (GPLv2+) WITHOUT ANY WARRANTY.
#

include $(top_srcdir)/Makefile.common

AM_CPPFLAGS	+= -I$(top_builddir) -I$(top_srcdir)

## libraries
lib_LTLIBRARIES	= libpacemaker.la

## SOURCES

libpacemaker_la_LDFLAGS	= -version-info 1:0:0

libpacemaker_la_CFLAGS	= $(CFLAGS_HARDENED_LIB)
libpacemaker_la_LDFLAGS	+= $(LDFLAGS_HARDENED_LIB)

libpacemaker_la_LIBADD	= $(top_builddir)/lib/pengine/libpe_status.la \
			$(top_builddir)/lib/cib/libcib.la \
			$(top_builddir)/lib/lrmd/liblrmd.la
# -L$(top_builddir)/lib/pils -lpils -export-dynamic -module -avoid-version
# Use += rather than backlashed continuation lines for parsing by bumplibs.sh
libpacemaker_la_SOURCES	=
libpacemaker_la_SOURCES	+= pcmk_sched_allocate.c
libpacemaker_la_SOURCES += pcmk_sched_bundle.c
libpacemaker_la_SOURCES += pcmk_sched_clone.c
libpacemaker_la_SOURCES += pcmk_sched_constraints.c
libpacemaker_la_SOURCES += pcmk_sched_graph.c
libpacemaker_la_SOURCES += pcmk_sched_group.c
libpacemaker_la_SOURCES += pcmk_sched_messages.c
libpacemaker_la_SOURCES += pcmk_sched_native.c
libpacemaker_la_SOURCES += pcmk_sched_notif.c
libpacemaker_la_SOURCES += pcmk_sched_promotable.c
libpacemaker_la_SOURCES += pcmk_sched_transition.c
libpacemaker_la_SOURCES += pcmk_sched_utilization.c
libpacemaker_la_SOURCES += pcmk_sched_utils.c
libpacemaker_la_SOURCES += pcmk_trans_graph.c
libpacemaker_la_SOURCES += pcmk_trans_unpack.c
libpacemaker_la_SOURCES += pcmk_trans_utils.c
