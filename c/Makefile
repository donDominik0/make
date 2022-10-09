MCU = atmega328p
F_CPU = 16000000UL
CC = avr-gcc
OBJCOPY = avr-objcopy
CFLAGS = -std=c99 -Wall -g -Os -mmcu=${MCU} -DF_CPU=${F_CPU} -I.
PORT = /dev/ttyACM0
TARGET = main
SRC = *.c

PROGRAMMER = arduino 

.PHONY: all
all: compile link flash

.PHONY: compile 
compile:
	${CC} ${CFLAGS} -o ${TARGET}.bin ${SRC} -v

.PHONY: link 
link:
	${OBJCOPY} -j .text -j .data -O ihex ${TARGET}.bin ${TARGET}.hex -v

.PHONY: flash 
flash:
	avrdude -v -V -p ${MCU} -c ${PROGRAMMER} -P ${PORT} -b 115200 -D -U flash:w:${TARGET}.hex:i

.PHONY: clean
clean:
	rm -f *.bin *.hex




