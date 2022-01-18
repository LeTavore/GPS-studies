# GPS-studies
###  First using Ai-Thinker A9G GPRS GSM GPS Pudding - Part 1

In this section will be documented the studies of the Ai Thinker A9G GPRS GSM GPS Pudding module, showing the step-by-step to lauch the "IDE", burning the firmware, and setting up the environment, to test de communication, by AT commands.

First of all, the Ai-Thinker A9G is an IoT development board based on the A9G GPRS/GSM+GPS/BDS modul, useful in remote applicantios, where you must send location data to other devices. It contains GPS/AGPS and GPRS technology, supported by a quad-band GSM/GPRS module, as well as telephone and message, etc. For more introduction info, visit: https://docs.ai-thinker.com/en/gprs/a9g/boards.

1) **A pinout info of this board can be viewd below:** 
![image](https://user-images.githubusercontent.com/79606632/149950392-8d29a4f4-212a-41d4-a82f-f373c1d7408e.png)


2) To start using this module, it is imporant to read the docs to configure the board, which can be found in the official AI-Thinker Technology website.
 2.1) **Basic debugging: wiring** 
*Its it important to know that the development board uses AT commands to release or update the firmware.
![wire_Connection](https://user-images.githubusercontent.com/79606632/149953432-a812690b-8bbc-4820-866b-e38ad53a4b15.jpeg)
Pay attention to the TX/RX connection! 
On the image above, it is possible to see the GPS antenna (square), GPRS antenna (small and rectangular), the A9G board and the FT232RL chip (USB-TTL converter).
When debugging, you must connect the Vsub-5V, GND-GND, At_TX-RX and At_RX-TX, remenbering that this connection is made  on the board to a USB-TTL connector, jumpers, and UBS-microUSB cables

2.2)  **Basic debugging: Power**
You can use a lithium battery ou a USB cable for power supply. 

3) Burning the firmware:
*Example of AT commands: https://docs.ai-thinker.com/gprs/examples
-Preparation: 
     -GPRS series module firmware release: http://docs.ai-thinker.com/gprs/firmware
     -Burning software download and burning tutorial: http://docs.ai-thinker.com/gprs_download
     -CSDK_Github open source information: https://github.com/Ai-Thinker-Open/GPRS_C_SDK
     -A9 Tracker app: A9Tracker app user guide
