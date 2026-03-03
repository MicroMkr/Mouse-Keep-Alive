You can flash the firmware using the following online tool: https://thelastoutpostworkshop.github.io/ESPConnect/

ESPConnect is a zero‑installation web application that runs entirely in a modern Chromium‑based browser (Chrome, Edge, Brave, etc.) and lets you explore, manage, back up, and flash firmware on ESP32/ESP8266 boards straight from the browser — no Python, no command‑line, no desktop tools required.

🔌 What You’ll Need

A Chromium‑based browser (Chrome, Edge, Brave, etc.) up to date.

An ESP32 board connected to your computer with a USB cable that has data lines (not just charging‑only).

Your firmware file in .bin format ready to upload (you can download it fromthis github).

📡 How to Flash Firmware Using ESPConnect

Open ESPConnect in your browser
Go to the web app page:
https://thelastoutpostworkshop.github.io/ESPConnect/

Connect Your Board
– Click the “Connect” button in the interface.
– Your browser will prompt you to choose the serial port. Pick the one your ESP is on.
– If your board doesn’t automatically enter bootloader mode, follow the on‑screen instructions to hold BOOT while clicking Connect.

Open the Flash Tools Section
– Once connected, the navigation sidebar will unlock.
– Select “Flash” or “Flash Firmware” from the menu — this is where firmware uploading happens.

Load Your Firmware File
– Click the area/button to open a file dialog.
– Select the .bin firmware file you want to flash.
- select Erase entire flash before writing option box.
– Leave the Flash offset settings on 0x0.

Start Flashing
– Press the “Flash” button to begin.
– You’ll see a progress indicator. Wait until it completes.
– Don’t disconnect while it’s flashing; wait for the bar to fill and show success.

Disconnect and Reboot
– After flashing finishes, click “Disconnect” and reset your board (press RESET).
– Your new firmware should now run.
