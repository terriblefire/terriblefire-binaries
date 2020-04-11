

1. Flash the firmware here to your esp module using a programmer interface and software like esptool.py

For the latest instructions and firmware see this page.

https://github.com/martin-ger/esp_slip_router#building-and-flashing

I dont update his page with those instructions because its duplicating effort. Just do what esp_slip_router says. My kid can do this with his raspberry pi so dont look for complications. There are none.

Windows can flash these modules with https://github.com/nodemcu/nodemcu-flasher. 

YOU NEED BOTH FIRMWARE FILES. Dont ask which one to flash. Its both and at the the addresses in the firmware. 

2. Then follow the instructions on the esp_slip_router page to setup you wifi settings.

3. Then install Roadshow or the roadshow demo on your amiga. 

4. Then unpack the zip file on your Amiga and EXECUTE install_script.

DO NOT MESS WITH THE IP SETTINGS NO MATTER WHAT MORONS ON A1K.ORG/EAB SAY. 

You Amiga's IP address will always be 192.168.240.2 and there will exist a 2 machine LAN between your Amiga and the ESP. Its IP address will always be 192.168.240.1

The ESP will have an IP address on your LAN/WIFI network that it obtains by DHCP. The ESP is an actual router in this situation and will do NAT for you. RTFM on the esp_slip_router page to understand how to configure this NAT. 

Dont bother looking for other slip.device's etc. Its utterly pointless unless you hit an issue between your ESP and your Amiga. SLIP is about as simple as possible and drivers arent going to make much of a difference to the performance. 

Since we have reports that 115200 works on CD32 i've updated the baud rate settings in the script but if you are using an A500 and doing this with a different type of machine you may want to try 38400. 
