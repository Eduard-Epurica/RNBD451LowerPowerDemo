# RNBD451LowerPowerDemo

Uses an MCP9808 temperature sensor to send data via the I2C communication protocol.

![image](https://github.com/Eduard-Epurica/RNBD451LowerPowerDemo/assets/64744850/23816491-ff99-404d-9bdc-96d59ef1ba95)

Built around an 8-bit microcontroller host (PIC18F47Q10) which processes the sensor data, converts it to decimal values and sends it over Transparent UART to the phone running MBD (Microchip Bluetooth Data).
The user has the ability to track the data in the Smart Dicover application in real time.
Both the host, and the module, are configured through register commands to run in the lowest power consumption setting.

![image](https://github.com/Eduard-Epurica/RNBD451LowerPowerDemo/assets/64744850/6f47239b-9167-4d09-93a0-0080b104369b)

The application is built on the existing MCP9808 driver using the MCC Melody framework. 
The RNBD451 uses a custom driver designed around the built in uart commands stored in it's internal flash
