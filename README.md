# CrowPanel HW V1.3 — Demo for P4 v1.0

Windows firmware installation package for **Elecrow CrowPanel Advanced
ESP32-P4 9-inch and 10.1-inch HW V1.3 panels**, 1024x600.

## Download

[Download the Windows package](./CrowPanelHW1.3_P4v3_Demo_for_P4_v1.0.zip)

## Compatibility

This package targets **ESP32-P4 silicon v3.1/v3.2**. PCB HW V1.3 and the
processor revision are separate: confirm the chip revision from the existing
working firmware's flashing/boot log before installation.
Do not use on P4 v1.x, 5-inch panels, or earlier PCB revisions.

Built with **ESP-IDF 5.5.4**. Firmware compilation succeeded. This is a test
candidate; Windows launch and HW V1.3 display/touch operation still require
validation. The existing flasher EXE is reused unchanged with esptool 5.3.1.

## Flashing

1. Download and fully extract `CrowPanelHW1.3_P4v3_Demo_for_P4_v1.0.zip` into a short local path.
2. Confirm the panel has P4 silicon v3.1/v3.2.
3. Connect the panel's **UART0 USB-C port** to Windows with a data-capable cable.
4. Close other applications using the COM port.
5. Run `CrowPanel_P4_fast_flasher.exe` from the extracted folder.
6. Select the COM port; click **Refresh** if necessary.
7. For the first installation over the previous firmware, enable
   **Clean install (erase entire flash)**. This deletes the previous P4
   firmware and settings; retain its recovery package before proceeding.
8. Click **Flash panel** and wait for **Firmware installed successfully**.
9. Do not disconnect the panel during installation. It restarts afterward.

Keep the EXE, `_internal`, and `firmware` directories together. All three
binaries come from one V1.3 build; do not mix files from other packages.

## Tester feedback

Test the 9-inch and 10.1-inch panels separately. Report chip/PCB revisions,
UART0 boot output at 115200 baud, backlight, image/colors, touch at the corners,
brightness adjustment, and behavior after a power cycle. Check animations and
audio together. Successful flashing does not confirm LCD operation.

## Troubleshooting

Use UART0, close applications holding the COM port, reconnect and click
**Refresh**. Do not bypass processor-revision errors or force flashing.
