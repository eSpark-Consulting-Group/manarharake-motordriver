## Project Description
The project involves being able to control DC Motors using an MCU and also uses FSRs. The PCB is expected to accept input commands over UART from a host system.

## Project Requirements
1. The hardware is powered with 7.4v battery. The battery is not rechargeable, it will be replaceable.
2. The hardware should be able to drive 6 Motors along with being able to read from the encoder. Datasheet for motor is attached [motor datasheet.pdf](https://github.com/eSpark-Consultants/manarharake-motordriver/files/13066469/motor.datasheet.pdf)
3. The hardware should also have 5 FSRs. Link to FSRs is here [FSR Sparkfun](https://www.sparkfun.com/products/9673).
4. Original choice for the MCU by client was the SoC used in Teensy 4.1 but it is most likely out of stock or NRND now. This needs to be rechecked but if not available, then the alternate MCU recommended by client is **MIMXRT106SDVL6B**.
5. The hardware should allow for sending commands via UART from a host system (or host MCU)
6. There should be means to save Encoders last value in case of power outage. For example, if the encoder was at "x" value and power gets cut, the system should be able to reboot from this same previous and drive from this points onwards and not from the start / reset. Please check if the encoder somehow directly supports this. If not, please see if having a small backup coin cell is sufficient or we would need some other means such as SD card etc?

### PCB Requirements
1. The PCB should be 5cm x 4cm in dimensions
