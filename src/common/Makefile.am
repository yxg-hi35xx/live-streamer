## Process this file with automake to produce Makefile.in


AM_CPPFLAGS = \
	-I$(top_srcdir)/src -I$(srcdir) -I$(builddir) \
	$(DBUSXX_CFLAGS)

if ENABLE_OSD
AM_CPPFLAGS += \
	$(FREETYPE_CFLAGS) \
	$(FONTCONFIG_CFLAGS) \
	$(SDL_CFLAGS)
endif

AM_CFLAGS = -Wall
AM_CXXFLAGS = -Wall


noinst_LTLIBRARIES =  \
	libcommon.la

libcommon_la_SOURCES =  \
	media-common.cpp \
	media-common.h \
	media-element.cpp \
	media-element.h \
	media-stream.cpp \
	media-stream.h \
	video-source.cpp \
	video-source.h \
	video-encoder.cpp \
	video-encoder.h \
	audio-source.cpp \
	audio-source.h \
	audio-encoder.cpp \
	audio-encoder.h

if ENABLE_OSD
libcommon_la_SOURCES += \
	video-osd.cpp \
	video-osd.h
endif
