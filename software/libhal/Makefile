MMDIR=../..
include $(MMDIR)/software/include.mak

OBJECTS=brd.o dmx.o font8x16.o mem.o pfpu.o snd.o time.o tmu.o ukb.o usb.o vga.o vin.o

all: libhal.a

libhal.a: $(OBJECTS)
	$(AR) clr libhal.a $(OBJECTS)
	$(RANLIB) libhal.a

$(MMDIR)/softusb-input/softusb-input.h:
	$(MAKE) -C $(MMDIR)/softusb-input

.PHONY: clean depend $(MMDIR)/softusb-input/softusb-input.bin

depend: $(MMDIR)/softusb-input/softusb-input.h
	makedepend -Y -- $(CFLAGS) -- *.c

clean:
	rm -f *.o libhal.a .*~ *~ Makefile.bak softusb-input.h

# DO NOT DELETE

brd.o: ../../software/include/base/stdlib.h
brd.o: ../../software/include/base/stdio.h
brd.o: ../../software/include/base/string.h
brd.o: ../../software/include/base/version.h
brd.o: ../../software/include/base/board.h ../../software/include/hw/sysctl.h
brd.o: ../../software/include/hw/common.h
brd.o: ../../software/include/hw/capabilities.h
brd.o: ../../software/include/hal/brd.h
dmx.o: ../../software/include/base/stdio.h
dmx.o: ../../software/include/base/stdlib.h ../../software/include/hw/dmx.h
dmx.o: ../../software/include/hw/common.h ../../software/include/hal/dmx.h
mem.o: ../../software/include/base/stdio.h
mem.o: ../../software/include/base/stdlib.h
mem.o: ../../software/include/base/malloc.h ../../software/include/hal/mem.h
pfpu.o: ../../software/include/base/stdio.h
pfpu.o: ../../software/include/base/stdlib.h
pfpu.o: ../../software/include/base/irq.h
pfpu.o: ../../software/include/base/system.h
pfpu.o: ../../software/include/hw/interrupts.h
pfpu.o: ../../software/include/hw/pfpu.h ../../software/include/hw/common.h
pfpu.o: ../../software/include/hal/pfpu.h
snd.o: ../../software/include/base/stdio.h
snd.o: ../../software/include/base/stdlib.h ../../software/include/base/irq.h
snd.o: ../../software/include/base/system.h ../../software/include/hw/ac97.h
snd.o: ../../software/include/hw/common.h
snd.o: ../../software/include/hw/interrupts.h
snd.o: ../../software/include/hw/sysctl.h
snd.o: ../../software/include/hw/capabilities.h
snd.o: ../../software/include/hal/snd.h
time.o: ../../software/include/base/stdio.h
time.o: ../../software/include/base/stdlib.h
time.o: ../../software/include/base/irq.h ../../software/include/base/board.h
time.o: ../../software/include/hw/sysctl.h ../../software/include/hw/common.h
time.o: ../../software/include/hw/interrupts.h
time.o: ../../software/include/hal/time.h
tmu.o: ../../software/include/base/stdio.h
tmu.o: ../../software/include/base/stdlib.h ../../software/include/base/irq.h
tmu.o: ../../software/include/base/board.h
tmu.o: ../../software/include/hw/interrupts.h
tmu.o: ../../software/include/hw/sysctl.h ../../software/include/hw/common.h
tmu.o: ../../software/include/hw/capabilities.h
tmu.o: ../../software/include/hw/tmu.h ../../software/include/hal/brd.h
tmu.o: ../../software/include/hal/tmu.h
ukb.o: ../../software/include/base/stdio.h
ukb.o: ../../software/include/base/stdlib.h
ukb.o: ../../software/include/base/console.h ../../software/include/hal/usb.h
ukb.o: ../../software/include/hal/ukb.h
usb.o: ../../software/include/hw/softusb.h ../../software/include/hw/common.h
usb.o: ../../software/include/hw/sysctl.h
usb.o: ../../software/include/hw/capabilities.h
usb.o: ../../software/include/hw/interrupts.h
usb.o: ../../software/include/base/uart.h ../../software/include/base/irq.h
usb.o: ../../software/include/base/stdio.h
usb.o: ../../software/include/base/stdlib.h ../../software/include/hal/usb.h
usb.o: input-comloc.h ../../softusb-input/softusb-input.h
vga.o: ../../software/include/base/stdio.h
vga.o: ../../software/include/base/stdlib.h
vga.o: ../../software/include/base/string.h
vga.o: ../../software/include/base/console.h
vga.o: ../../software/include/base/system.h ../../software/include/base/irq.h
vga.o: ../../software/include/hw/interrupts.h ../../software/include/hw/vga.h
vga.o: ../../software/include/hw/common.h ../../software/include/hal/tmu.h
vga.o: ../../software/include/hw/tmu.h ../../software/include/hal/vga.h
vin.o: ../../software/include/base/stdio.h
vin.o: ../../software/include/base/stdlib.h ../../software/include/hal/vin.h
vin.o: ../../software/include/hw/bt656cap.h
vin.o: ../../software/include/hw/common.h
