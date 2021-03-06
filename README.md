# LoRaNode Examples

Examples to use LoRaWan with [LoraNode_1.3](https://github.com/marcobrianza/Lora_Node_1.3) hardware on The Things Network

## ttn-abp-LoraNode-button-serial
Basic example to use LoraNode   
Press the red buttton to send a packet  
monitor LMIC activity with the serial port

## ttn-abp-LoraNode-display
Example code to conficure and send a packet on ttn with LoraNode 1.3 + [OLED shield ](https://wiki.wemos.cc/products:d1_mini_shields:oled_shield)   
All the LoRaWan options are configurable: 

* Channel  
* Radio Power
* Spread Factor/Data Rate
* Port
* Data Lenght
* TX data payload
* Acknowledgment

press the black button to select the item  
the red button to change value  
Select "->" and press the Red button to send the message.


## ttn-abp-LoraNode-temperature
This example sends every 60 seconds a temperature value on ttn  
A one Wire DS18B20 temperature sensor is required.  
To temperature decode data in the ttn backend use this [payload function](https://github.com/marcobrianza/_ttn-functions/blob/master/ttn_float_decoder.js) in the "payload formats" of the [ttn console](https://console.thethingsnetwork.org/). The output json with add the field with the temperature value.


## ttn-abp-LoraNode-mapper
Example code to map ttn coverage [https://ttnmapper.org/](https://ttnmapper.org)

an app running on a mobile phone is need to log message position  
[ttn mapper Android](https://play.google.com/store/apps/details?id=com.jpmeijers.ttnmapper)  
[ttn mapper iOS](https://itunes.apple.com/us/app/ttn-mapper/id1128809850?mt=8) (not working for me at this time)

For complete functionality the WeMos OLED display is required.  
Set the parameters by the ui (the standard ones should be ok)  
Set "->" to 1 and move around :-)  
The DT number (interval of packet transmission) will be x10 by the code. The standard =1 =10s