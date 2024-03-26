# ModbusMAT ![ModbusMAT](https://github.com/fortiko/ModbusMAT/assets/1612534/2f1f153d-f40f-488c-864a-9013ce28fb57)

(Note: just a convenience mirror of ataytugal.com ModbusMAT freeware ModBus program)

Source: https://web.archive.org/web/20141216195755/http://ataytugal.com/

In my intensive use of modbus protocol in engineering applications, I had to use various modbus protocol test programs. In general this programs were helpful. However, in some cases, some  extra functionalities are needed. Therefore, I decided to make my own modbus test program.

ModbusMAT is my Modbus test program for the system integrators. The project is freeware. However, it is one the most functional modbus test programs.

Considering the flexibility for the future, I have used C++ language,  written all serial classes and modbus classes individually and  not used any serial or modbus component from a third party company.

## Download
[ModbusMAT 1.1.zip](https://github.com/fortiko/ModbusMAT/raw/main/ModbusMAT%201.1.zip)

## CURRENT FUNCTIONALTY  

* Modbus RTU polls (0x01,0x02,0x03,0x04) with user friendly interface.
* Write single coil (0x05), write  multiple coils(0x0F), write single register (0x06), write multiple registers (0x10) functions are implemented.
* Data traffic monitoring with colored text.
* Write your own frame functionality : Frames can  be written in hexadecimal ASCII characters.
* CRC calculator and adder for user frames
* Display and write values in formats : Signed, unsigned, binary, float, float inversed, long, long inversed
* Independent data conversions calculator ( Convert signed integer, unsigned integer, long integer, long integer inversed, floating point, floating point  inversed formats to each other.)
* Search address functionality ( If the user don't know valid addresses in a device, ModbusMAT tries to find one, using a fast find algorithm )

