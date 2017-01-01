# rc-switch  ***  Note this was originally written for Arduino so ignore all Arduino references except where I have added 'IDE'
Use your Arduino IDE to discover remote radio controlled devices


This will most likely work with all popular low cost power outlet sockets, namely SC5262 / SC5272, HX2262 / HX2272, PT2262 / PT2272, EV1527, RT1527, FP1527 or HS1527 chipset. Also supports Intertechno outlets any many more including the Ozzie Bunnings RC sockets.

##Receive and decode RC codes

Find out what codes your remote is sending. Use your remote to control your ESP8266-12-e nodeMCU to discover them.

All you need is a Arduino IDE with ESP8266-12e nodeMCU attached, a 315/433MHz AM receiver attached to ESP8266-12e on pin D3 and the remote hand set.
