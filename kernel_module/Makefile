obj-m += fb_st7796s.o
obj-m += fb_ili9488.o
obj-m += ili9488.o

PWD := $(shell pwd)

all: default

default:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules

install:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules_install

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean