# STM32 ile Sıcaklık ve Nem Değerini Okuma 


## STM32F103C8T6
STM32F103C8T6 is a 32-bit microcontroller manufactured by STMicroelectronics having ARM Cortex-M3 Architecture. CPU frequency is 72 Mhz. 

## DHT11

DHT11 temperature and humidity sensor can measure temperature between 0-50°C and ± 2°C accuracy, and humidity value between 20-80% with 5% accuracy. On the sensing side there is a humidity sensing component along with an NTC temperature sensor.

The ions are released as water vapor is absorbed by the substrate, which increases the conductivity between the electrodes. The change in resistance between the two electrodes is proportional to the relative humidity. Higher relative humidity reduces the resistance between the electrodes, while lower relative humidity increases the resistance between the electrodes.

They consist of a temperature and humidity sensor and an NTC temperature sensor / thermistor to measure temperature. A thermistor is a thermal resistor. It is a resistor that changes its resistance t temperature. Technically, all resistors are thermistors. Their resistance changes depending on the increase and decrease in temperature. However, the change is often very small and difficult to measure. Thermistors are manufactured in a way that makes the resistance change noticeable.

## LM35
The LM35 temperature sensor, which is used to measure the temperature of the environment, is a temperature sensor with analog output. The LM35 temperature sensor output voltage changes in direct proportion to the temperature. The temperature measurement range varies between -55 and 150 degrees. It can measure with 0.5 degree precision when it is fed with a voltage value between 4-30 V and with a current of less than 60 microamperes. The output value changes by 10mV for each degree.

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

## References
[DHT11](https://vidieukhien.xyz/2018/04/06/bai-12-tim-hieu-va-giao-tiep-stm32f4-voi-dht11/ )
[ADC Usage with STM32]( https://medium.com/@mehmetgkk/stm32-ile-adc-kullan%C4%B1m%C4%B1-19d78eb05097)
[STM32CubeIDE](https://www.youtube.com/watch?v=TCrmxJuvzyY&t=3s ) 
[Sending Data with USART](https://www.youtube.com/watch?v=1vipR-6nJaQ )

