# TinyGS
Configure TinyGS on the Domino4 xChips:
- Follow the [TinyGS](https://tinygs.com) instructions.
- Configure your own board with this JSON line:
```JSON
{"name":"[433] <YOUR GROUND STATION NAME>","aADDR":60,"oSDA":26,"oSCL":27,"oRST":0,"pBut":0,"led":0,"radio":1,"lNSS":15,"lDIO0":33,"lDIO1":0,"lBUSSY":0,"lRST":0,"lMISO":12,"lMOSI":13,"lSCK":14,"lTCXOV":0.0}
```

- If you compile using PlatformIO, then change upload speed to `upload_speed = 1000000`
- The OLED doesn't work out of the box, so you need to mod the code. I have [reported the problem to TinyGS](https://github.com/G4lile0/tinyGS/issues/146), where I also have posted the temporary solution.

## Antenna
- I plan to use this antenna [HYS 433Mhz 3dbi Omni Antenna 50 Ohm GSM Aerial W/3M(9.8ft) RG58 Coaxial Cable SMA Male Plug and Mounting Bracket](https://www.amazon.com/gp/product/B086YV2QLS) from Amazon, but other antennas would do find. Check out recommendations on the Telegram TinyGS Community chat
- But build a quadrifilar helicoidal [QFH](#QFH) antenna in the meantime

### QFH
- Calculator: http://jcoppens.com/ant/qfh/calc.en.php
- Downloaded .scad file from Thingiverse. TODO link.
