# TinyGS
## New Way since version 2403242
- Make sure you don't have the Serial port open in another app, such as Arduino
- Plug your core into a PPU (Power & Programmer USB-A) and an ODA (Output Display A)
- Open [The TinyGS Installer](https://installer.tinygs.com/) in Google Chrome (or Microsoft Edge)
- Click on "**Install**". Only release at time of writing is 2403242.
- A windows comes up where you can pair (if not already paired) your USB Device. Click "**Connect**"
- Click on "**INSTALL TINYGS**", _optionally_ check **Erase Device**, then "**NEXT**", then "**INSTALL**"
- After install is completed, you can _optionally_ click "**NEXT**", and then "**LOGS & CONSOLE**", then click "**RESET DEVICE**"
- Follow [This Guide](https://github.com/G4lile0/tinyGS/wiki/Ground-Station-configuration)
- Make sure you made note of your **latitude** and **longitude** (with 3 decimals ONLY), and your **MQTT Credentials**.
- Connect to the **My TinyGS** wifi
- Open [192.168.4.1](192.168.4.1) in your browser
- Config as per above, don't worry about board type, but add the below template after you changed your station name:

### CWV V4
```JSON
{"name":"[433] <Insert Your Ground Station Name Here>","aADDR":60,"oSDA":26,"oSCL":27,"oRST":-1,"pBut":0,"led":0,"radio":1,"lNSS":15,"lDIO0":33,"lDIO1":0,"lBUSSY":0,"lRST":0,"lMISO":12,"lMOSI":13,"lSCK":14,"lTCXOV":0.0}
```
### CWA V2
```JSON
{"name":"[433] <Insert Your Ground Station Name Here>","aADDR":60,"oSDA":17,"oSCL":18,"oRST":-1,"pBut":0,"led":40,"radio":1,"lNSS":35,"lDIO0":34,"lDIO1":0,"lBUSSY":0,"lRST":0,"lMISO":38,"lMOSI":37,"lSCK":36,"lTCXOV":0.0}
```

## More setup
- In Telegram go to **@tinygs_personal_bot**
- Type "**/weblogin**", this will give you a one liner login (save it)
- Click on the link and update your settings:
  - Describe your setup, maybe add some links.
  - Take a picture of your setup and upload it.


## Antenna
- Suggested antenna [HYS 433Mhz 3dbi Omni Antenna 50 Ohm GSM Aerial W/3M(9.8ft) RG58 Coaxial Cable SMA Male Plug and Mounting Bracket](https://www.amazon.com/gp/product/B086YV2QLS) from Amazon, but other 433MHz antennas would do fine. Check out recommendations on the Telegram TinyGS Community chat
- If you use an antenna with SMA, like the one above, you also need [an SMA to a U.Fl/IPEX converter](https://www.amazon.com/gp/product/B01HXU1PKS)

### DIY QFH Antenna 
Or build a quadrifilar helicoidal antenna...
- Download [OpenSCAD](https://openscad.org)
- Download [QFH .scad file](https://www.thingiverse.com/thing:634205)
- Use this [calculator](http://jcoppens.com/ant/qfh/calc.en.php) to get the parameters for your 433MHz version
- Use the parameters from the calculator in the .scad file, and then use OpenSCAD to generate a .stl, which you 3D print. Add wire and etc as per suggestion...
