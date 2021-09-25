# CP2104_GPIO_CTRL
Key steps:
1. make 
2. cp cp210x.ko to /lib/modules/<kernel-version>/kernel/drivers/usb/serial
3. insmod /lib/modules/<kernel-version/kernel/drivers/usb/serial/usbserial.ko
4. insmod /lib/modules/<kernel-version/kernel/drivers/usb/serial/cp210x.ko
  
Notes:
  ls /dev/ttyUSB* to check the device status.
  lsmod |grep cp2104
  sudo rmmod cp2104
  sudo modprobe cp2104
  lsmod |grep cp2104
  
  may need to uninstall before install:
  sudo rmmod cp210x
