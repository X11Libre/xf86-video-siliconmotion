#  Copyright 2005 Adam Jackson.
#
#  Permission is hereby granted, free of charge, to any person obtaining a
#  copy of this software and associated documentation files (the "Software"),
#  to deal in the Software without restriction, including without limitation
#  on the rights to use, copy, modify, merge, publish, distribute, sub
#  license, and/or sell copies of the Software, and to permit persons to whom
#  the Software is furnished to do so, subject to the following conditions:
#
#  The above copyright notice and this permission notice (including the next
#  paragraph) shall be included in all copies or substantial portions of the
#  Software.
#
#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
#  FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT.  IN NO EVENT SHALL
#  ADAM JACKSON BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
#  IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
#  CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

# this is obnoxious:
# -module lets us name the module exactly how we want
# -avoid-version prevents gratuitous .0.0.0 version numbers on the end
# _ladir passes a dummy rpath to libtool so the thing will actually link
# TODO: -nostdlib/-Bstatic/-lgcc platform magic, not installing the .a, etc.

AM_CFLAGS = $(XORG_CFLAGS) $(CWARNFLAGS) $(PCIACCESS_CFLAGS)

siliconmotion_drv_la_LTLIBRARIES = siliconmotion_drv.la
siliconmotion_drv_la_LDFLAGS = -module -avoid-version
siliconmotion_drv_ladir = @moduledir@/drivers

siliconmotion_drv_la_SOURCES = \
         compat-api.h \
         regsmi.h \
         smi_501.c \
         smi_501.h \
         smi_accel.c \
         smi_exa.c \
         smi_dac.c \
         smi_driver.c \
         smi.h \
         smi_i2c.c \
	 smi_pcirename.h \
         smi_video.c \
         smi_video.h \
	 smi_crtc.h \
	 smi_crtc.c \
	 smilynx_crtc.c \
	 smi_output.c \
	 smilynx_output.c \
	 smilynx_hw.c \
	 smilynx.h \
	 smi501_crtc.c \
	 smi501_output.c
