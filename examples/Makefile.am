INCLUDES = -I$(top_srcdir)/libusb
LDADD = ../libusb/libusb-1.0.la
noinst_PROGRAMS = listdevs

listdevs_SOURCES = listdevs.c

if HAVE_SIGACTION
dpfp_SOURCES = dpfp.c
noinst_PROGRAMS += dpfp

if THREADS_POSIX
dpfp_threaded_SOURCES = dpfp_threaded.c
dpfp_threaded_CFLAGS = $(THREAD_CFLAGS) $(AM_CFLAGS)
noinst_PROGRAMS += dpfp_threaded
endif
endif
