#Daisy X., Yunie Y., Abby S.
export ARCH=arm
export CROSS_COMPILE=arm-linux-gnueabihf-
ccflags-y := -std=gnu99

obj-m += lcd2.o
obj-m += gamespace.o

# Kernel source directory
KDIR =/tmp/guest-1eipom/Documents/group14/lab3/bb-kernel/KERNEL

PWD = $(shell pwd)

default:
	$(MAKE) -C $(KDIR) SUBDIRS=$(PWD) modules
clean:
	$(MAKE) -C $(KDIR) SUBDIRS=$(PWD) clean
