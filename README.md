## Dual Antenna Setup  

This uses **two NRF24 modules** connected to the ESP32 via **separate SPI buses**:  

- **HSPI** (High-Speed SPI) – First NRF24 module  
- **VSPI** (Default SPI) – Second NRF24 module  

By using two independent transceivers, the system can operate on different **2.4 GHz channels simultaneously**, providing:  
- **Wider frequency coverage**  
- **More effective interference testing**  
- **Dynamic channel switching** (alternating between random and sequential modes every 3 seconds)  

⚠️ **Note:** This setup requires proper wiring of both SPI buses and should only be tested in a **controlled environment**.  
