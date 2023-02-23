# rpi-workstation
raspberry pi zero w - make it a developers workstation<br>
https://lamsworkshop.blogspot.com/p/raspberry-pi-zero-w-make-it-developers.html

sample main.cpp for PIC32MX250F128D:
```
#include <xc.h>

const int devcfg3 __attribute__((section(".config_BFC00BF0"))) = 0x8FFFFFFF;
const int devcfg2 __attribute__((section(".config_BFC00BF4"))) = 0xFFF979D9;
const int devcfg1 __attribute__((section(".config_BFC00BF8"))) = 0xFF74CDDB;
const int devcfg0 __attribute__((section(".config_BFC00BFC"))) = 0x7FFFFFFB;

int main(void) {
  LATBSET = TRISBCLR = 0x200;
  while(1);
}
```

Ardunio:
```
wget https://github.com/dgtie/rpi-workstation/raw/main/avr.tar.gz
```
Attiny414:
```
wget https://github.com/dgtie/rpi-workstation/raw/main/attiny.tar.gz
```
#Stm32f103:
```
wget https://github.com/dgtie/rpi-workstation/raw/main/stm32.tar.gz
```
