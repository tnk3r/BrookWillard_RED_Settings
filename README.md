# BrookWillard_RED_Settings
![Alt text](overlays_small.jpg?raw=true "Overlays")
![Alt text](ipp2_luts_small.jpg?raw=true "IPP2 LUTS")

This ZIP file includes my default camera preset, default monitor overlays, and renamed versions of RED's "IPP2" REC709 LUTs.

* NOTE: There are some bugs in the current release build [as of 8/1/18] which will affect loading these presets.

* NOTE: This preset was built on a DSMC2 Monstro camera. As such you should double-check your ISO and Resolution settings after applying the preset. The settings in the preset may be inappropriate for your camera.

To install:

•	Copy the “luts”, “presets”, and “overlays” folders into the root directory of a formatted REDmag. Insert the REDmag into a camera.

•	Open MENU - IMAGE - 3D LUT - IMPORT/EXPORT… and copy all LUTs to the camera. Close the menu.

•	Open MENU - OVERLAYS - CUSTOM and copy all overlays to the camera. Close the menu.

•	Open MENU - PRESETS and copy the “Cinema” preset to the camera. DO NOT APPLY THE PRESET WHEN PROMPTED. Close the menu.

•	Manually apply the “Cinema” preset. THIS WILL TAKE LONGER THAN USUAL - think 30 seconds. Let it do its thing until it hasn’t done anything for 10-15 seconds.

•	Open MENU - IMAGE - IMAGE PIPELINE and manually change “Color Space” to REDWideGamutRGB” and “Gamma Curve” to “Log3G10”. These settings do not populate properly in the current release build.

•	Open MENU - MONITORING - MONITORS and go through each monitor output individually. Due to a bug in the current release build only certain monitor settings will have carried from the preset. Generally you must change “Display Preset” to “3DLUT”. Your “Overlay” may be incorrect as well. NOTE that due to another bug “3D LUT” will not be selectable if the actual LCD or EVF in question is not currently plugged in.

•	Open MENU - 3D LUT [now a shortcut in the lower-left] and choose your preferred LUT. RED’s current default LUT is “C2R2” but my preferred LUT is the Light Iron Color 2 FILM LUT which I did not seek permission to distribute.

NOTE - As of the current DXL2 firmware [available 8/1/18], any LUTs intended for the DXL2 are designed with a +1 stop compensation built in to them. For your camera sensitivity to behave properly on a RED DSMC2 camera you must UNCHECK “Use Updated ISO calibration” in MENU - IMAGE - ISO. This is ONLY relevant if you are planning on using DXL2 LUTs with +1 stop compensation in a DSMC2 camera.

NOTE - The three SDI overlays have slightly different content. “Cinema SDI 1080P” is the cleanest overall. “Cinema SDI 1080P TLS” has RED’s “traffic light” clipping indicators added in the lower left as a sneaky way to keep an eye on exposure at video village. I have also swapped timecode and timecode status position to balance the overlay with this change. Finally, “Cinema SDI 1080P EXP” has both the “traffic lights” and RED’s Luma Histogram enabled. This is for those who don’t want to lose the functionality of these features but who can’t stand to stare at RED’s touch screen user interface all day. Remember that these overlays can be used on any display. I’ve found the “Cinema SDI 1080P EXP” overlay to be useful on the Touch LCD with “Auto Hide Menus” enabled for those who want a larger image and cleaner interface on the touch screen but still want to see the Histogram without having to manually touch it.

NOTE - My preset has “Enable Reduced Judder Preview” enabled in MENU - MONITORING - ADVANCED. This is the similar to Arri’s “Smooth Mode” - it shows your preview at a higher frame rate which reduces the perceived image delay for the camera operator. On certain bodies this can reduce UI performance and in extreme circumstances can result in a crash. If you do not like this feature, turn it off.

NOTE - HD-SDI frequency is set to match timebase in my preset. If you would like to reduce frame delay over HD-SDI you can change the SDI frequency to 59.94Hz. Be sure to test this, as not all accessories [Preston Light Ranger II most notably] support 1080p 59.94.

Use and distribute this collection as you see fit, just give credit where it is due.

Enjoy,

~Brook Willard, 8/1/18
