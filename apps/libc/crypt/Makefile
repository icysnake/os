################################################################################
#
#   Copyright (c) 2015 Minoca Corp. All Rights Reserved
#
#   Module Name:
#
#       Crypt Library
#
#   Abstract:
#
#       This module contains the crypt library, which contains the C library
#       functions like crypt, encrypt, fcrypt, and setkey.
#
#   Author:
#
#       Evan Green 6-Mar-2015
#
#   Environment:
#
#       User Mode C Library
#
################################################################################

BINARY = libcrypt.so.1

BINARYTYPE = so

BINPLACE = bin

ENTRY := 0

INCLUDES += $(SRCROOT)/os/apps/libc/include;

OBJS = crypt.o          \

DYNLIBS = $(BINROOT)/libc.so.1           \

include $(SRCROOT)/os/minoca.mk

postbuild:
	@mkdir -p $(BINROOT)/skel/lib
	@cp -p $(BINROOT)/$(BINARY) $(BINROOT)/skel/lib

