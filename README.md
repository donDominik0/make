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
curl -LJO https://github.com/donDominik0/make/blob/main/arduino-cli/blink/Makefile
```
Attach board, compile and upload code
```bash
make all
```
Remove build files
```bash
make clean
```
