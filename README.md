Libsub configuration and example code in linux :
Install libsub
Install libusb-1.0-0-dev
Instead of:
#include <libusb/libusb.h>
do:
#include <libusb.h>
gcc example.c `pkg-config --libs --cflags libusb-1.0`
Below example is using c++, so use 
	g++ example.c `pkg-config --libs --cflags libusb-1.0`

Note :
 pkg-config --libs --cflags libusb-1.0
 -I/usr/include/libusb-1.0 -lusb-1.0 


2. Refrence 
https://www.beyondlogic.org/usbnutshell/usb6.shtml

Gives a short intro into usb

