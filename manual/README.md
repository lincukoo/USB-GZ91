# Product Introduction  
This is a universal Zigbee USB Dongle. It can be used as a Zigbee gateway in Home Assistant, openHAB, Zigbee2MQTT, or other open-source platforms to locally control all your Zigbee devices, so you don’t need to invest in different brands’ Zigbee hubs.  
![1732784837_goods_img](https://github.com/user-attachments/assets/56c0566f-bfcf-4a61-899e-2cbe3ad77dae)

# Quick Setup  
There are two ways to use the Zigbee USB Dongle to manage your Zigbee devices on Home Assistant: ZHA or Zigbee2MQTT (please note that the dongle can only work in one way at the same time). and it will be similar settings on other platforms.  

Note：Before setup device, you need make sure the Home Assistant system has been installed on host device (such as Raspberry Pi). Connect your computer to the same Wi-Fi as the Raspberry Pi and enter the address into your browser to open the Hass page as below:  

http://x.x.x.x:8123 (x.x.x.x is the IP address of home assistant)  

## 1.	ZHA(Zigbee Home Automation)  
① Insert the dongle and add ZHA Integration  
<img width="606" height="352" alt="image" src="https://github.com/user-attachments/assets/afb6cd9d-bfb7-4402-9abd-d39cb10a069d" />  
<img width="503" height="234" alt="image" src="https://github.com/user-attachments/assets/9e357a4a-fd34-4538-aaa2-cbb3ea9ae448" />  
② Configuration for the dongle:  
Serial Device Path: /dev/ttyUSB0 - USB Serial  
Detail configuration, please refer below:  
<img width="389" height="287" alt="image" src="https://github.com/user-attachments/assets/b0224b38-e41f-43f1-a715-b2915adb4023" />  
<img width="517" height="438" alt="image" src="https://github.com/user-attachments/assets/6b0298b1-85cf-4f5d-a5ab-79b623ea290b" />  
<img width="404" height="451" alt="image" src="https://github.com/user-attachments/assets/6db261bc-e2e8-44bb-97bc-d344f610edb4" />  
<img width="403" height="351" alt="image" src="https://github.com/user-attachments/assets/6de3ca7e-0157-42bd-9b15-464afd997ac2" />  
③ Add sub-devices to the gateway dongle,refer as below:  
<img width="606" height="359" alt="image" src="https://github.com/user-attachments/assets/5d5d3047-7048-4d77-925b-707824cc09ec" />  
<img width="606" height="263" alt="image" src="https://github.com/user-attachments/assets/04cb56b0-8238-4939-b39f-cea60cf9c36a" />  
<img width="606" height="162" alt="image" src="https://github.com/user-attachments/assets/b474b856-3c54-4965-8ca2-4a61ae641b6c" />  
<img width="606" height="430" alt="image" src="https://github.com/user-attachments/assets/6a534b4f-c13a-4147-ab9f-f73c06dce4c3" />  
<img width="532" height="512" alt="image" src="https://github.com/user-attachments/assets/7f3d8106-b012-4d54-bf08-1c42bc1788af" />  
## 2.	Zigbee2MQTT  
Note 1:  
If you don't have an MQTT broker yet; in Home Assistant go to Settings → Add-ons → Add-on store and install the Mosquitto broker add-on, then start it.  
Note 2:  
Go back to the Add-on store, click ⋮ → Repositories, fill in
https://github.com/zigbee2mqtt/hassio-zigbee2mqtt and click Add → Close.  
① Insert the dongle and add Zigbee2MQTT add-ons  
<img width="605" height="360" alt="image" src="https://github.com/user-attachments/assets/5c972538-00e8-432c-8141-9b590b9d4626" />  
<img width="605" height="277" alt="image" src="https://github.com/user-attachments/assets/679b5679-bb2d-41ab-8c77-129e2a814b84" />   
<img width="605" height="213" alt="image" src="https://github.com/user-attachments/assets/e1f541e9-3a82-48a2-96b7-6b76b8a4678c" />  
<img width="606" height="183" alt="image" src="https://github.com/user-attachments/assets/50e2b5d2-0f1d-431a-970d-3e8f3c502ff1" />  
② Configuration for the dongle:  
mqtt:  
base_topic: zigbee2mqtt  
server: mqtt://192.168.2.142:1883 (the IP address of the mqtt server)   
user: mqtt (username of the mqtt server)  
password: mqtt (password of the mqtt server)  
client_id: zigbee2mqtt  
serial:  
port: /dev/ttyUSB0  
adapter: ember  
<img width="605" height="247" alt="image" src="https://github.com/user-attachments/assets/790e0692-ff18-4bc1-8ddd-e0a3dc921f64" />  
<img width="605" height="221" alt="image" src="https://github.com/user-attachments/assets/e40ea90e-6313-45e5-b939-390ea64b54bc" />  
<img width="606" height="286" alt="image" src="https://github.com/user-attachments/assets/a32e3791-b136-440b-8828-d830a4912627" />  
③ Add sub-devices to the gateway dongle,refer as below:  
<img width="606" height="279" alt="image" src="https://github.com/user-attachments/assets/994c29ec-deec-4af6-9a08-1f7f74e22bd4" />  
<img width="605" height="271" alt="image" src="https://github.com/user-attachments/assets/d40e2c3e-c0fe-4168-8a55-3f317ff9784d" />  
<img width="605" height="225" alt="image" src="https://github.com/user-attachments/assets/9409e261-8906-4b26-bd7d-8178e5f48a47" />




















