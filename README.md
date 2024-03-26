# ModbusMAT ![ModbusMAT](https://github.com/fortiko/ModbusMAT/assets/1612534/2f1f153d-f40f-488c-864a-9013ce28fb57)

(Note: just a convenience mirror of ataytugal.com ModbusMAT freeware ModBus program)

Sources: 
* https://web.archive.org/web/20141216195755/http://ataytugal.com/
* https://web.archive.org/web/20150202131544/http://www.ataytugal.com/ModbusMat.htm

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

## INSTRUCTIONS
ModbusMAT is easy to use. Mainly, it has 3 tab sheets. Also, the Conversions Calculator is included.

### Connection
Click on the 1st item at the tool bar at top. Choose or fill  the appropriate parameters. Close the form. Click on 2nd item at the top toolbar to open port. You can see your connection status at "Read Status" at bottom.

![01Comm](https://github.com/fortiko/ModbusMAT/assets/1612534/00d1cef2-9314-49cb-a4d6-2ebf0745ffcb)

### Polling
Choose "Modbus Poll" tab sheet. Fill or choose the suitable parameters on the left and press "Start Polling" button. Values will be seen on the right side according to format you choose.

![02Poll](https://github.com/fortiko/ModbusMAT/assets/1612534/e6d7c299-0851-4b24-9df1-e687bba55b57)

### Write to Registers
Double-click on the address you want to write on. A form will pop up. Write the desired value and click on "Write Value" button.

![03WriteFloat](https://github.com/fortiko/ModbusMAT/assets/1612534/d9436ef4-e51b-4600-bee0-ae5c18662400)

### Write to Coils
Double-click on the address you want to write on. A form will pop up. Choose the desired value and click on "Write Value" button.

![04WriteCoil](https://github.com/fortiko/ModbusMAT/assets/1612534/0c60b7ec-e0e8-4193-9679-79ed23fca119)

### Create your Frame and Send
Choose the "Extra" tab sheet. Write the frame you want to send. (Writing format is not important. Non-Hex characters will be ignored.) When a frame is entered, the "CRC bytes" box re-calculates a new 16-bit CRC value. Click on "Add CRC button if you want to add calculated CRC block. "Click on the "Send" button. If you want to send the same frame continuously, click on the "Send Continuously" button.

![05Create](https://github.com/fortiko/ModbusMAT/assets/1612534/d7b95595-49dd-4679-9654-e5ce5c6ae4c6)

### Search Valid Address
Choose "Extra" tab sheet. Choose or fill the search parameters to characterize your search. Finally, click on the "Start Search" button.

![06Search](https://github.com/fortiko/ModbusMAT/assets/1612534/a335d160-18da-443e-86d6-22ff4535b7bf)

### Search Results
When a valid response is received the search stops. Looking at "Write Status" at the bottom the valid address can be understood.

![07Search2](https://github.com/fortiko/ModbusMAT/assets/1612534/83669727-0adf-49ad-959f-380fab9cedd5)

### Communication Monitor
Choose "Comm Monitor" tab sheet to view the port activity in colored display.

![08Monitor](https://github.com/fortiko/ModbusMAT/assets/1612534/a3ba56ee-9136-456c-b91e-4f81a1ed277d)

### Conversions Calculator
Click on the "Conversions Calculator" item at the top toolbar. "Conversions" form will pop up. Choose a format and write value in the edit box. Below the edit box the corresponding hexadecimal value will be displayed.

![09Conv1](https://github.com/fortiko/ModbusMAT/assets/1612534/2bf9dd72-d5f5-4d35-b9e9-ecf5284f924c)

When another format is choosen the value will be converted. The value below edit box does not change unless a new value is entered.

![10Conv2](https://github.com/fortiko/ModbusMAT/assets/1612534/7842bc1b-143d-4074-b065-9f78d84e6b42)

 


  

  

  

  

  

 
 
