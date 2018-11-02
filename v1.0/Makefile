
PWD := $(shell pwd)

ARCH=arm
CC=~/b288/lichee/out/sun8iw10p1/linux/common/buildroot/external-toolchain/bin/arm-linux-gnueabi-gcc
KERNELDIR := ~/b288/lichee/linux-3.10/
obj-m := kmsg_drv.o
.PHONY: all clean

all:
	@echo -e "\e[0;32;1m--Compiling 'kmsg drv'...\e[0;36;1m" 
	@echo -e "\e[0m" 
	@$(MAKE) -C $(KERNELDIR)  M=$(PWD) modules

clean:
	$(MAKE) -C $(KERNELDIR) M=$(PWD) modules clean
