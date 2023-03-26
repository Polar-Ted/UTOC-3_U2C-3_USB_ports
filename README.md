# Understanding the UTOC/U2C USB A ports
There has bit of misunderstang in regards to the UTOC-3/U2C-3 USB A ports.  
First off the USB-A ports on the BTT U2C-3 and the Mellow Fly UTOC-3 are not a USB hub and can't be configured to work as one. 

The USB-A ports are intended to allow devices that are capabile of comunicaton by CAN bus protocol but lack a CAN transciever to join a CAN bus network. 
This would include mot fo the STM32 CPUs and RP2040 devices that have avaliable open GPIO pins to connect as RX/TX to the CAN transciever. 

![U2C-3  USB-A Schematic](images/u2c_usb_a_schematic.png)

Each of the 2 USB-A ports ( top and bottom) has it's own CAN transciever IC, a jumper for a 120 ohm resistor to terminate the CAN bus and a +5V jumper to supply power out of the USB-A to to the device conected to it. 
 - BTT U2C-3      
   ![U2C-3](https://github.com/bigtreetech/U2C/blob/master/Image/pinout.png)      


 - [Mellow Fly UTOC-3](https://mellow-3d.github.io/fly-utoc_pins.html)       
   ![UTOC-3](https://mellow-3d.github.io/images/fly-utoc/fly_utoc-pins.png)      

## Links

 - [Big Tree Tech U2C Github ](https://github.com/bigtreetech/U2C)
 - [Mellow UTOC Github](https://mellow-3d.github.io/fly-utoc_general.html)
 
