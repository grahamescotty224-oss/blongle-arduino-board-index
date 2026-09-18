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

Current platform version: **1.0.1**

## Source and licence

BLONGLE SAMD Boards is based on Adafruit ArduinoCore-samd 1.7.17. Upstream
copyright and licence notices remain in the platform source.

This repository is distributed under the GNU Lesser General Public License
v2.1. See [LICENSE](LICENSE).

## Updating and duplicate board entries

Use Boards Manager to update **BLONGLE SAMD Boards** to 1.0.1. Select
**BLONGLE-MC1-NANO** under **BLONGLE SAMD Boards**, not the older
**BLONG SAMD Boards** manual installation.

If both appear, first confirm the new package uploads and runs your sketch.
Then quit Arduino IDE and move the old `blong` folder out of your sketchbook's
`hardware` directory into a backup folder outside the sketchbook. On the original
macOS setup it is `~/Documents/Arduino/hardware/blong`. Restart the IDE.
Renaming the folder inside `hardware` does not remove it from discovery.
Keep the working bootloader archive; this update does not require reflashing it.

## Changes in 1.0.1

- Fix the HID USB endpoint narrowing warning with an explicit byte conversion.
- Preserve the earlier variant, Serial, linker and 8 KB bootloader-space fixes.
- Keep 1.0.0 in the index for rollback.
- Add release checks for these fixes and duplicate-installation guidance.

The 1.0.0 package was installed, compiled, uploaded and run on the owner's Mac
and MC1-NANO. That is not a claim of testing every operating system or library.
