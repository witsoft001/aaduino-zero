BINARY = main

ROOT = $(shell git rev-parse --show-toplevel)
COMMON = $(ROOT)/common
CFLAGS = -I. -I$(COMMON)

OBJS = \
    $(COMMON)/tmp102.o \
    $(COMMON)/sw_i2c.o \
    $(COMMON)/rfm69.o \
    $(COMMON)/spi_driver.o \
    $(COMMON)/spiflash.o \
    $(COMMON)/hw.o \
    $(COMMON)/event.o \
    $(COMMON)/ringbuf.o \
    $(COMMON)/tick.o \
    $(COMMON)/dbg_printf.o \
    $(COMMON)/mini-printf.o

#    past.o \

include $(ROOT)/libopencm3.target.mk

bmpflash:
	./bmp-flash.sh
