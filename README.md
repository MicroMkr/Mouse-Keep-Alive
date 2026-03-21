<img width="577" height="866" alt="ChatGPT 2" src="https://github.com/user-attachments/assets/830bf35c-5a63-4ded-a91b-755358497245" />

The ESP32S3 Mouse Keep-Alive is a small hardware device that prevents your computer from going idle by emulating real mouse activity. Built on the ESP32-S3, it appears to the computer as a standard USB mouse and periodically generates tiny cursor movements to keep the system active.

Unlike software solutions, this device works as a fully hardware-based mouse emulator, so it does not require installing any software on the computer.

The device includes a built-in Wi-Fi web interface, allowing you to easily configure its behavior directly from your phone, tablet, or PC browser. Through the web UI you can adjust movement intervals, enable or disable activity, and customize the operation to suit your needs.

<img width="1024" height="1536" alt="Mouse Keep-Alive interface with cartoon mouse" src="https://github.com/user-attachments/assets/d3c89112-36be-4436-ba22-4774859cb7b9" />


**Installation:**

Flashing ESP Firmware Using the Espressif Web Flash Tool

This guide explains how to flash firmware to an ESP device using Espressif’s browser-based flashing tool.

**Requirements**

A computer with Google Chrome or Microsoft Edge

A USB cable connected to your ESP board

The compiled firmware file (.bin)

1. Open the Web Flash Tool

Open the following page in your browser:

https://espressif.github.io/esptool-js/

This tool runs directly in the browser and does not require installing any software.

2. Connect the ESP Device

Connect your ESP board to the computer using a USB cable.

Click the Connect button on the web page.

A window will appear showing available serial ports.

Select the COM port corresponding to your ESP device (USB JTAG/serial debug unit (COM xx) - Paired

Click Connect.

3. Set the Flash Address and Firmware File

In the Flash Address field, enter:

0x0

Click Choose File.

Select your firmware .bin file.

Example configuration:

Address	File
0x0	firmware.bin


4. Optional Settings (Recommended)

Before flashing, enable:

Erase Flash – This clears any previous firmware and prevents compatibility issues.

Leave other settings at their default values unless specific changes are required.

Typical defaults:

Flash Mode: Keep

Flash Size: Keep

Baud Rate: 460800 or 921600

5. Enter Bootloader Mode (Only If Required)

Many ESP boards enter flashing mode automatically.

If flashing fails, manually enter bootloader mode:

Hold the BOOT button.

Press and release the RESET button.

Release the BOOT button.

The board is now ready for flashing.

6. Flash the Firmware

Click Program.

The flashing process will begin.

Example console output:

Erasing flash...
Writing at 0x00000000...
Hash verified.
Hard resetting via RTS pin...

Wait until the process completes.

7. Finish

After flashing is finished:

Press the RESET button on the ESP board (if it does not reboot automatically).

The new firmware will start running.
