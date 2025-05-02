# STM32-SSD1306-OLED
Programming STM32 with SSD1306 OLED display using HAL code stm32cube firmware

## Referensi
- https://github.com/ARM-software/CMSIS_4/tree/master
- https://github.com/afiskon/stm32-ssd1306
- https://github.com/eblot/newlib/tree/master

[**Interface SSD1306 OLED display with STM32**](https://controllerstech.com/oled-display-using-i2c-stm32/)

[**(YT)Interface SSD1306 OLED display with STM32**](https://youtu.be/M5ddTjrcvEs?si=K2IlHJ6ADH_gAWyI)

## Setting Compiler
- Buka file c_cpp_properties.json
- Ubah compilerPath jadi /usr/bin/arm-none-eabi-gcc
- Sesuaikan IncludePath
- Test compile program dengan make

## Mengatasi Error core_cm3.h
- Jika ada error: core_cm3.h: No such file or directory
- Download firmware CMSIS_4 >> [**Download CMSIS_4**](https://github.com/ARM-software/CMSIS_4)
- Copy File core_cm3.h atau semua file dari CMSIS_4 "CMSIS_4/CMSIS/Include"
- Paste file yang dicopy ke "Drivers/CMSIS/Device/ST/STM32F1xx/Include"
- Test compile program dengan make
- Pastikan tidak ada error

## Tips Compiler
Sebelum compile tulis path library pada MakeFile

Contoh :

Core/Src/fonts.c \

Core/Src/ssd1306.c \

## Bitmap Dsplay
Bitmap Generator Png to Bitmap Script: https://javl.github.io/image2cpp/

buat Header .h file > /Core/Inc/ bitmap.h