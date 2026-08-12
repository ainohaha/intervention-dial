# Intervention Dial

Web Bluetooth receiver for a rotary-dial thought logger
(Arduino UNO R4 WiFi + KY-040 encoder).

Click the dial to mark a noticed thought, turn it to rate intensity 0–10,
click again to confirm. This page shows the level live and keeps a local log.

The **board** is the logger: every confirmed event is written to its EEPROM
before transmission, so nothing is lost if the phone locks, the browser
closes, or Bluetooth drops. This page is a viewer that collects whatever it
hasn't seen yet, and supplies the clock so events get real timestamps.

## Use

Open this page in a Web Bluetooth browser — **Bluelight** or **Bluefy** on
iOS, Chrome on Android/desktop. Safari does not support Web Bluetooth.

## Privacy

Logged events are stored only in this browser's `localStorage` on your own
device. Nothing is uploaded, and this repository contains no personal data.

Firmware lives alongside this page in the project it was built for.
