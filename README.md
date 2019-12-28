# Esp32MicroWebSrv

.bin for ESP32 to test MicroWebSrv in AP mode 

SSID Esp32Peacock
192.168.4.1

add /get?test1=value1&test2=value2 to test GET method

use microPython V 1.9.4 to Solve ampdu ignore deleting tx error

http://micropython.org/resources/firmware/esp32-idf3-20180511-v1.9.4.bin

# How to flash
- Erase Flash
python esptool.py -p com5 erase_flash
- Write bin
python esptool.py -p com5 -b 115200 write_flash -z  0x0000 Esp32MicroWebSrv.bin


https://microwebsrv.hc2.fr/

https://github.com/jczic/MicroWebSrv
