Реализован счетчик энергии по воде. Позволяет настроить начальное значение (в литрах) и на основании его производит отсчет по входу 27. Выход 26 позволяет подключить индикатор.

Перед использованием файловой системы, после установки микропитона, запустить один раз(следующую группу комманд:
**import os**
**os.umount('/')
os.VfsFat.mkfs(bdev)**
**os.mount(bdev, '/')**
это необходимо, для создания файловой системы FAT



Используемое оборудование

ESP32-WROOM-32U с прошивкой `esp32-20220117-v1.18`

XY-K485

Меркурий 230 APT-03 CN



Подключение Меркурий <-> XY-K485

A+ - 19

B- - 24

Подключение XY-K485

GND - GND

RXD - 16

TXD - 17

VCC - 3.3V

Питание на счетчик

L - 10

N - 7

Питание интерфейса счетчика 12VDC

+12VDC - 23

-12VDC - 18

