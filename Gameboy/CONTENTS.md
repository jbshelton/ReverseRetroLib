### Before you start
I haven't 100% confirmed that everything I made is 100% accurate to measurements and working, however I think with how much time I spent on everything the measurements should be pretty sound- but take that with a grain of salt. There are a few things that will be updated in some time, but their current state is fine for this release:
- Fix footprint for IR LED and phototransistor (make a regular 2-pad footprint that just has to be placed twice)
- Add "tutorial" of sorts for assembling the cartridge adapter
- Clean up and add FreeCAD source file I used to make the board outlines so others can tweak it easier

---

### Included files
The resources that I have included in this repository are:
- Board outlines for both the OEM board and the custom board outline I used, which omits the hole for the voltage regulator board and the DC jack mounting hole
- Footprints for the buttons/battery terminals, power switch, IR LEDs, volume wheel, and cartridge slot
- PCB files for my GBA SP to GBC cartridge slot adapter and model for the 3D printable mounting bracket
- Symbols for the CGB CPU and KF2007/KF2005 CPUs in the style of the original GBC schematic (which Gekkio's symbol does not match)

---

### Required/recommended external files
- For the cartridge slot, I used [William Durand's KiCad libs](https://github.com/willdurand/kicad-libs)
- For the CPU (PCB footprint), RAM, link port, etc. you'll need [Gekkio's KiCad libs](https://github.com/Gekkio/gekkio-kicad-libs), or make your own
- 3D model for the [PJ307 headphone jack](https://grabcad.com/library/pj-307-stereo-connector-1)

---

### Note for KF200x clone CPUs
On the KF2007, pin 39 needs to be tied to the 3.3 volt rail for normal operation. If tied to ground (not sure about floating,) the screen will be shifted vertically. The pinout is the same as the CGB CPU, so the only difference is tying that one pin high.

On the KF2005, the pinout on the bottom right hand corner of the chip is shifted slightly, so it's pin 44 instead of 39. The KF2005 is the GBC clone CPU found only on the older, non-backlit models of GB Boy Colour that also have infrared. It does not have the same pinout as the KF2007. I did get the pinout by analyzing the chip without taking it off the board, but did not make a test/repro board to confirm it, so use it at your own risk.
