# CrowPanel Demo for P4

Demo firmware for **Elecrow CrowPanel Advanced ESP32-P4 panels with 1024 × 600 touch displays**.

## Download

Choose the package matching both the processor silicon revision and audio hardware.
PCB hardware revision and processor silicon revision are different identifiers.

| Panel | Windows package |
| --- | --- |
| HW1.3, P4 v1.0-v1.99, legacy audio | [Download P4 v1.x Demo](./CrowPanel_HW1.3_ESP32P4_V1.x_Demo_NoColorProbe.zip) |
| New audio batch, P4 v3.1/v3.2, ES8311 + ES7210 + NS4263B | [Download P4 v3.x Demo](./CrowPanel_P4_V3.x_ES8311_ES7210_Demo.zip) |

## Flashing

1. Download and fully extract the matching ZIP from the table above.
2. Connect the panel’s **UART0 USB-C port** to a Windows computer using a data-capable USB cable.
3. Open the extracted folder.
4. Run `CrowPanel_P4_fast_flasher.exe`.
5. Select the panel's COM port. Click **Refresh** if the port is not listed.
6. **Clean install** erases the entire flash and saved settings. Leave it unchecked when updating a compatible Demo package; use it only when you intend a full clean installation.
7. Click **Flash panel**.
8. Do not disconnect the panel while flashing.
9. Wait for the **Firmware installed successfully** message.

The panel restarts automatically after flashing.

## Troubleshooting

If the panel is not detected, reconnect it through UART0, close any application using the COM port, and click **Refresh**.
