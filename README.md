# Make

## Arduino-CLI

### Install arduino-CLI

Create sketch with command
```bash
arduino-cli sketch new <sketchname> 
```
Enter sketch directory
```bash
cd <sketchname>
```
Add Makefile
```bash
curl -O https://raw.githubusercontent.com/donDominik0/make/main/arduino-cli/blink/Makefile
```
Attach board, compile and flash code
```bash
make all
```
Remove build files
```bash
make clean
```


## AVR-GCC and AVRDUDE

### Install avr-gcc and avrdude

Create new \*.c file
```bash
touch <filename>.c
```

Add Makefile
```bash
curl -O https://raw.githubusercontent.com/donDominik0/make/main/c/Makefile
```

Compile, link and flash code
```bash
make all
```

Remove build files
```bash
make clean
```
