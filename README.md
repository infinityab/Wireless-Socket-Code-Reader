# rc-switch 

Use your Arduino IDE to discover remote radio controlled devices

This will most likely work with all popular low cost power outlet sockets, namely SC5262 / SC5272, HX2262 / HX2272, PT2262 / PT2272, EV1527, RT1527, FP1527 or HS1527 chipset. Also supports Intertechno outlets any many more including the Ozzie Bunnings RC sockets.

##Receive and decode RC codes

Find out what codes your remote is sending. Use your remote to control your ESP8266-12-e nodeMCU to discover them.

All you need is a Arduino IDE with ESP8266-12e nodeMCU attached, a 315/433MHz AM receiver attached to ESP8266-12e on pin D3 and the remote hand set.

** Further note - when I discovered all my ON and OFF codes for my pack of 3 sockets I found that to get it to work I had to set and additional MS bit to get it to work, this is not as compilcated as it sounds, so if you have a similar problem try this.

Use the decimal codes that are received in my example 1425377058 for one of the codes. Use the MS calcualtor in scientific mode set to DECIMAL and copy the number in. Then switch to HEX mode and note the hex digits, 54F58722 in this case. The upper MS HEX number is 5 or 0101 in binary, so we need to ADD or OR in a MS 1000 or 8 in hex. So on the calculator hit the + sign and enter in hex 80000000 and = and the answer in the example should be D4F58722, then switch calculator back to DECIMAL and the result is the code you will use 3572860706 - easy peasy!
