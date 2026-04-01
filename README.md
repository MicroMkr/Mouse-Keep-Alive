<img width="577" height="866" alt="ChatGPT 2" src="https://github.com/user-attachments/assets/830bf35c-5a63-4ded-a91b-755358497245" /> 

The ESP32S3 Mouse Keep-Alive is a small hardware device that prevents your computer from going idle by emulating real mouse activity. Built on the ESP32-S3, it appears to the computer as a standard USB mouse and periodically generates tiny cursor movements to keep the system active.

Unlike software solutions, this device works as a fully hardware-based mouse emulator, so it does not require installing any software on the computer.

The device includes a built-in Wi-Fi web interface, allowing you to easily configure its behavior directly from your phone, tablet, or PC browser. Through the web UI you can adjust movement intervals, enable or disable activity, and customize the operation to suit your needs.

<img width="1024" height="1536" alt="Mouse Keep-Alive interface with cartoon mouse" src="https://github.com/user-attachments/assets/d3c89112-36be-4436-ba22-4774859cb7b9" />


**Installation:**

Flashing ESP Firmware Using the MicroMaker dedicated Web Flash Tool:

https://micromkr.github.io/firmware/MicroMaker-Flasher.html

Connect your ESP32-S3

Choose the Mouse Keep-Alive firmware

Press Connect device - choose your device

Press flash firmware

**7. Finish**

After flashing is finished:

Press the RESET button on the ESP board (if it does not reboot automatically).

The new firmware will start running.
