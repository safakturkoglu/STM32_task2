# STM32 ile Sıcaklık ve Nem Değerini Okuma 


## STM32F103C8T6
STM32F103C8T6 is a 32-bit microcontroller manufactured by STMicroelectronics having ARM Cortex-M3 Architecture. CPU frequency is 72 Mhz. 

## Software

- STM32CubeMX
- Keil IDE
- Proteus

## STM32CubeMX and Keil IDE
We open the CubeMX software and click on the new project and select the microcontroller as STM32F103C6. We selected the GPIO Output pins. Then double click on the STM32F103C8 at the right panel. Next, a new window will be opened where you need to change SYS Debug to Serial Wire and RCC of High-Speed Clock or HSC to Crystal/Ceramic Resonator. Clock configuration is set 72 Mhz. A code is generated according to our choices. Keil is also an IDE where we can edit the code produced for us. We are making additions to the main code. After editing the code, we build. Then the .hex is generated.

## Proteus
To reach the outputs, the required circuit is established. The .hex is embedded in the MCU part of the established circuit. Then it is run. Outputs are also displayed thanks to the Visual Terminal.
#### Proteus Circuit
![Proteus_Circuit](https://user-images.githubusercontent.com/95358360/146682793-bc1a62d1-aaf1-4755-821e-92d1ff18602d.PNG)
#### Visual Terminal
![Visual Terminal](https://user-images.githubusercontent.com/95358360/146683176-0ebf93d8-74d5-4965-a658-8d8d9d2550c5.png)

#### LEDs
In the LED Indicator part, it is decided which color the LED will light up, thanks to the temperature measurement in the DHT11. It may light up red, yellow and green depending on the conditions.

![leds](https://user-images.githubusercontent.com/95358360/146683502-9124d593-377d-4e25-ba47-9a4ffec1601a.PNG)


