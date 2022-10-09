CC = arduino-cli
PORT = /dev/ttyACM0


# attach board, compile and upload code
.PHONY:all
all: attach compile flash


# attach board to port
.PHONY: attach 
attach:
	${CC} board attach -p ${PORT} -v


# compile code
.PHONY: compile
compile:
	${CC} compile -ve


# upload code
.PHONY: flash
flash:
	${CC} upload -v


# clean all
.PHONY: clean
clean:
	rm -r build *.json


