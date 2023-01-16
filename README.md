# rs485 communication with RS485 to TTL module

* Sending and receiving data is done in **"rs485_communication_rxtx"**. Data receiving was carried out with the polling method, and data sending was carried out with the interrupt method.

* In **"uart_dma_stm32f103"**, data retrieval was performed by DMA method. For the project of importing data with dma, after selecting usart1 asynchronous in the pinout section, it is necessary to add the USART1_RX option by clicking Add in the DMA setting section. Mode Normal, Memory, Data Width Byte will be made. And then it is necessary to enable USART1 global interrupt in NVIC setting.


<img src="https://github.com/ozgedurgut/rs485_communication_rxtx/blob/main/rs485_communication_rxtx/1.jpg"   >
<img src="https://github.com/ozgedurgut/rs485_communication_rxtx/blob/main/rs485_communication_rxtx/2.jpg"   >
