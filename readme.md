This is a Hotas project based on a STM32 Nucleo L432KC (works with pretty much every FS USB capable stm32 board I think, but you'll need to regenerate project files using cubeMX for your board)

Some files might not be up to date, like the stm32cubeMX file may have differents pinout than the stm3232cubeIDE project 

JoyTest.h is the HID descriptor, and the .ioc file is the cubeMX file

The hid descriptor is copied in Middlewares/ST/STM32_USB_Device_Library/Class/HID/Src/usbd_hid.c and the device type (nInterfaceProtocol) is changed to 0x04 (joysick) in the same file.
