include $(top_srcdir)/build/modmake.rulesam
MODNAME=mod_openh264

OPENH264_DIR=/usr/local/

mod_LTLIBRARIES = mod_openh264.la
mod_openh264_la_SOURCES  = mod_openh264.cpp
mod_openh264_la_CXXFLAGS   = $(AM_CXXFLAGS) -I$(OPENH264_DIR)/include/wels
mod_openh264_la_LIBADD   = $(switch_builddir)/libfreeswitch.la
mod_openh264_la_LDFLAGS  = -L$(OPENH264_DIR)/lib/ -lopenh264 -avoid-version -module -no-undefined -shared
