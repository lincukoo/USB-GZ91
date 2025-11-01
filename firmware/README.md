Use any tool that supports sending XMODEM, Here uses “Tera Term” as example.   

1.Insert the dongle into the USB port of PC, Open "Tera Term", select the serial port of the dongle. The port can be viewed in the Device Management Console.  
<img width="370" height="216" alt="image" src="https://github.com/user-attachments/assets/83842fdd-fc4e-4666-9ef7-a1f82e765f46" />  
Setup the serial port’s parameter and click “New setting”:  
<img width="373" height="305" alt="image" src="https://github.com/user-attachments/assets/dded646f-9e3f-4dcb-8cc9-f47e240bfb10" />  
<img width="370" height="363" alt="image" src="https://github.com/user-attachments/assets/5071b737-77fa-4e05-992e-84ed5042e591" />  
2.Dongle Enter Bootloader Mode.   
Keep pressing the Boot button, restart the device, and release the Boot button after Dongle enters the serial port Bootloader, then enter 1.  
<img width="394" height="321" alt="image" src="https://github.com/user-attachments/assets/c9d275b5-8a9b-4acd-90e1-065e71349cb4" />  
3.Click “File->Transfer->XMODEM->Send…”, select local downloaded firmware. [Click here to down](https://github.com/lincukoo/USB-Dongle/tree/main/firmware)   
Note: You should complete this step before the end of the progress bar displayed as the character "C". Otherwise, an error will be reported, and you need to re-enter 1.  
<img width="392" height="391" alt="image" src="https://github.com/user-attachments/assets/40de9a17-0944-4dad-8b3b-d61093c551c0" />  
4.Download completed when it shows the progress in 100%.  
<img width="287" height="220" alt="image" src="https://github.com/user-attachments/assets/6dd5d82d-9a5a-4328-9a24-02cac81c789d" />  
5.Re-plug the dongle to run with new firmware.






