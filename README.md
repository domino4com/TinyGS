# TinyGS
Configure TinyGS on the Domino4 xChips:
- Follow the [TinyGS](https://tinygs.com) instructions.
- Configure your own board with this JSON line:
```JSON
{"name":"[433] <YOUR GROUND STATION NAME>","aADDR":60,"oSDA":26,"oSCL":27,"oRST":0,"pBut":35,"led":21,"radio":1,"lNSS":15,"lDIO0":33,"lDIO1":21,"lBUSSY":21,"lRST":18,"lMISO":12,"lMOSI":13,"lSCK":14,"lTCXOV":0.0}
```
- I use this antenna [HYS 433Mhz 3dbi Omni Antenna 50 Ohm GSM Aerial W/3M(9.8ft) RG58 Coaxial Cable SMA Male Plug and Mounting Bracket](https://www.amazon.com/gp/product/B086YV2QLS) from Amazon, but other antennas would do find. Check out recommendations on the Telegram TinyGS Community chat
- If you compile using PlatformIO, then change upload speed to `upload_speed = 1000000`
- 

