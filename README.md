# GBC Reproduction Library
I created this repository in order to share some of the resources I created while working on my own GBC reproduction circuit board, which will be available soon! Everything was designed to be used with KiCad 6.

---

### Before you start
I haven't 100% confirmed that everything I made is 100% accurate to measurements and working, however I think with how much time I spent on everything the measurements should be pretty sound- but take that with a grain of salt. There are a few things that will be updated in some time, but their current state is fine for this release:
- Fix footprint for IR LED and phototransistor (make a regular 2-pad footprint that just has to be placed twice)
- Add "tutorial" of sorts for assembling the cartridge adapter
- Add FreeCAD source file I used to make the board outlines so others can tweak it easier

---

### Included files
The resources that I have included in this repository are:
- Board outlines for both the OEM board and the custom board outline I used, which omits the hole for the voltage regulator board and the DC jack mounting hole
- Footprints for the buttons/battery terminals, power switch, IR LEDs, volume wheel, and cartridge slot
- PCB files for my GBA SP to GBC cartridge slot adapter and model for the 3D printable mounting bracket

---

### Required/recommended external files
- For the cartridge slot, I used [William Durand's KiCad libs](https://github.com/willdurand/kicad-libs)
- For the CPU, RAM, link port, etc. you'll need [Gekkio's KiCad libs](https://github.com/Gekkio/gekkio-kicad-libs), or make your own
- 3D model for the [PJ307 headphone jack](https://grabcad.com/library/pj-307-stereo-connector-1)

---

### When's this GBC repro coming out?
At the moment (July 26th,) I have finished the first prototypes for my Ultra Boy Color PCB, as well as finished the design for the revision 2 PCB which I will be selling via my [Ko-fi page](https://ko-fi.com/reverseretro), either as a DIY kit or assembled board. I estimate that I'll be ready to sell them by mid-August.
