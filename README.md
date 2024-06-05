# TinyGS
## New Way since version 2403242
- Open [The TinyGS Installer](https://installer.tinygs.com/) in Google Chrome (other browsers might be supported)
- INSTALL TINYGS
- Follow [This Guide](https://github.com/G4lile0/tinyGS/wiki/Ground-Station-configuration)
- Make sure you made note of your lat and lon (with 3 decimals ONLY), and your MQTT Credentials.
- Connect to the **TinyGS** wifi
- Open [192.168.4.1](192.168.4.1) in your browser
- Config as per above, don't worry about board type, but add the below template after you changed your station name:
```JSON
{"name":"[433] <Insert Your Ground Station Name Here","aADDR":60,"oSDA":26,"oSCL":27,"oRST":-1,"pBut":0,"led":0,"radio":1,"lNSS":15,"lDIO0":33,"lDIO1":0,"lBUSSY":0,"lRST":0,"lMISO":12,"lMOSI":13,"lSCK":14,"lTCXOV":0.0}
```

## Antenna
- I plan to use this antenna [HYS 433Mhz 3dbi Omni Antenna 50 Ohm GSM Aerial W/3M(9.8ft) RG58 Coaxial Cable SMA Male Plug and Mounting Bracket](https://www.amazon.com/gp/product/B086YV2QLS) from Amazon, but other antennas would do find. Check out recommendations on the Telegram TinyGS Community chat
- If you use an antenna with SMA, like the one above, you also need an SMA to a U.Fl/IPEX converter, like this one: https://www.amazon.com/gp/product/B01HXU1PKS
- But build a quadrifilar helicoidal [QFH](#QFH) antenna in the meantime

### DIY QFH Antenna 
- Download [OpenSCAD](https://openscad.org)
- Download [QFH .scad file](https://www.thingiverse.com/thing:634205)
- Use this [calculator](http://jcoppens.com/ant/qfh/calc.en.php) to get the parameters for your 433MHz version
