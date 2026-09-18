# BLONGLE Arduino Board Index

Arduino Boards Manager support for the **BLONGLE-MC1-NANO**.

## Install

1. Install Arduino IDE 2.
2. Open **Arduino IDE > Settings** on macOS, or **File > Preferences** on
   Windows and Linux.
3. Add this URL under **Additional Boards Manager URLs**:

   `https://raw.githubusercontent.com/grahamescotty224-oss/blongle-arduino-board-index/main/package_blongle_index.json`

4. Open **Tools > Board > Boards Manager**.
5. Search for `BLONGLE`.
6. Install **BLONGLE SAMD Boards**.
7. Select **BLONGLE-MC1-NANO** and the board's USB port.

If an upload fails, press RESET twice quickly, select the new port and upload
again.

## Supported boards

- BLONGLE-MC1-NANO Rev A

## Included

- BLONGLE-MC1-NANO board definition and tested Rev A variant
- Adafruit SAMD 1.7.17 based Arduino core
- Correct 8 KB bootloader flash reservation
- RGB Welcome example
- Arduino, HID and native USB support

The Rev A bootloader retains the Adafruit Trinket M0 USB identity. It may
temporarily appear as `TRINKETBOOT` or `Adafruit Trinket M0` while entering
the bootloader.

## Release files

The package index is stored at the repository root. Platform archives are
attached to matching GitHub releases.

Current platform version: **1.0.0**

## Source and licence

BLONGLE SAMD Boards is based on Adafruit ArduinoCore-samd 1.7.17. Upstream
copyright and licence notices remain in the platform source.

This repository is distributed under the GNU Lesser General Public License
v2.1. See [LICENSE](LICENSE).
