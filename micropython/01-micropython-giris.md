# MicroPython
MicroPython, mikrokontrolcülerde ve kısıtlı ortamlarda çalışmak üzere Python 3.4 üzerine tasarlanan optimize bir uygulamadır.

Temel amacı mikrokontrolcülerde çalışmak olan MicroPython minimum 256KB ROM ve 16KB RAM'e ihtiyaç duymaktadır. Ayrıca **x86, x86-64, ARM, ARM Thumb, Xtensa** gibi pek çok yaygın işlemci mimarisinde de düzgün bir şekilde çalışabilmektedir.

C99 standartları ile yazılan MicroPython'ın çekirdek deposu ise MIT ile lisanslanmıştır. 

## Özellikleri 
- Pek çok derleme seçeneği içerir.
- Başlatma süresi oldukça kısadır.
- Basit ve güçlü bir bellek yönetimine sahiptir. 
- Bellek kullanımı aşıldığında *MemoryError* veya *RuntimeError* hatalarını döndürür.
- Python kodunu minimal bir biçimde yorumlar. 
- Hata ayıklamak basittir.
- [_thread](https://docs.micropython.org/en/latest/library/_thread.html) sınıfı sayesinde birden fazla iş parçacığıyla çalışmak kolaydır.
-  Thumb and Xtensa mimarileri için [*inline assembler*](https://en.wikipedia.org/wiki/Inline_assembler) desteği vardır.

## MicroPython Portlarına Sahip Bazı Platformlar

|                                 Platformlar                                    |
| :------------------------------------------------------------------------: |
|    [CC3200](https://www.ti.com/product/CC3200)          |
|    [ESP32](http://esp32.net/)        |
|    [ESP8266](http://esp8266.net/)                   |
|    [RP2040](https://datasheets.raspberrypi.org/rp2040/rp2040-datasheet.pdf)      |
|    [STM32](https://www.st.com/en/microcontrollers-microprocessors/stm32-32-bit-arm-cortex-mcus.html)  |
|    [Teensy](https://www.pjrc.com/teensy/)    |
|    [Zephyr](https://zephyrproject.org/)  |

### Ekstra İçerikler
|                                                   İçerikler                                                                            |
| :------------------------------------------------------------------------------------------------------------------------------------: |
| [Canlı Test](http://micropython.org/live/)                                                         |
| [Resmi Döküman](http://docs.micropython.org/en/latest/)                                                    |
| [İnceleme Videosu](https://www.youtube.com/watch?v=5LbgyDmRu9s) |

### Kaynakça
http://micropython.org/

https://github.com/micropython/micropython/tree/master/ports
