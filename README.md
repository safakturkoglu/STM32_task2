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


![proteus_circuit](https://user-images.githubusercontent.com/95358360/146682793-bc1a62d1-aaf1-4755-821e-92d1ff18602d.PNG)


