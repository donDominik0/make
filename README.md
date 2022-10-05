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
Attach board, compile and upload code
```bash
make all
```
Remove build files
```bash
make clean
```
