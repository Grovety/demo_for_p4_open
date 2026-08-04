# CrowPanel Demo for P4

Demo firmware preinstalled on **Elecrow CrowPanel Advanced ESP32-P4 panels with 1024 × 600 touch displays**.

This package provides a ready-to-use Windows flashing tool for hardware revision **V1.2**.

## Download

[Download the ready-to-use Windows package](./CrowPanelv1.2_Demo_for_P4_v1.1.zip)

## Flashing

1. Download and fully extract `CrowPanelv1.2_Demo_for_P4_v1.1.zip`.
2. Connect the panel’s **UART0 USB-C port** to a Windows computer using a data-capable USB cable.
3. Open the extracted folder.
4. Run `CrowPanel_P4_fast_flasher.exe`.
5. Select the panel's COM port. Click **Refresh** if the port is not listed.
6. Make sure **Clean install (erase entire flash)** is enabled.
7. Click **Flash panel**.
8. Do not disconnect the panel while flashing.
9. Wait for the **Firmware installed successfully** message.

The panel restarts automatically after flashing.

## Troubleshooting

If the panel is not detected, reconnect it through UART0, close any application using the COM port, and click **Refresh**.
