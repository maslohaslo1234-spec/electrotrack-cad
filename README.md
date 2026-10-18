# Electrotrack CAD

<img width="1348" height="893" alt="Zrzut ekranu 2026-10-18 102011" src="https://github.com/user-attachments/assets/66774ad2-af3f-4c55-b310-5494828e005e" />

This repository has the mechanical design of my Electrotrack project: the enclosure for the PCB and the parts of the circular track. I modelled everything in Onshape during Week 2 of Hack Club Half Life.

The electronics (schematic, PCB and firmware) are in a separate repository:

[Electrotrack electronics](https://github.com/maslohaslo1234-spec/electrotrack)

## Why I’m building it

Electrotrack is a small electromagnetic ball accelerator, and this is its mechanical side. I wanted to learn how to design parts around a real PCB: check where the components and connectors are, make them reachable from outside, and get the parts ready for a first test print.

## PCB enclosure

I designed the enclosure around the 100 × 83.5 mm PCB. I imported the PCB model into Onshape to check where the components and connectors end up. The enclosure has:

- A base with four posts for the PCB.
- Places for M3 heat-set inserts.
- A lid held with four screws.
- Mounting tabs on the outside, so it can be screwed to a plywood base.
- A window for the OLED.
- Openings for USB, connectors and wires.

## Track

So far I have the curved track segments, the coil formers and the IR sensor mounts. I put them together in one assembly in Onshape. Nothing is printed yet, so I don’t know how well the parts fit in real life.

## Files

### STEP models


| File | Description |
| --- | --- |
| [`pcb_enclosure.step`](cad/step/pcb_enclosure.step) | PCB enclosure |
| [`pcb_enclosure - base.step`](cad/step/pcb_enclosure%20-%20base.step) | Enclosure base |
| [`pcb_enclosure - lid.step`](cad/step/pcb_enclosure%20-%20lid.step) | Enclosure lid |
| [`track.step`](cad/step/track.step) | Track segment |
| [`coil.step`](cad/step/coil.step) | Coil formers |
| [`sensor module.step`](cad/step/sensor%20module.step) | IR sensor mount |

### STL models


| File | Description |
| --- | --- |
| [`pcb case - Case base.stl`](cad/print/stl/pcb%20case%20-%20Case%20base.stl) | Enclosure base |
| [`pcb case - lid.stl`](cad/print/stl/pcb%20case%20-%20lid.stl) | Enclosure lid |
| [`track.stl`](cad/print/stl/track.stl) | Track segment |
| [`coil.stl`](cad/print/stl/coil.stl) | Coil former |
| [`sensor module.stl`](cad/print/stl/sensor%20module.stl) | IR sensor mount |

### Project documentation

| File | Description |
| --- | --- |
| [`BOM.csv`](BOM.csv) | Funding and purchasing BOM from Half Life |
| [`JOURNAL.md`](JOURNAL.md) | Development journal from Half Life |
| [`LICENSE`](LICENSE) | Repository licence |


This is still a CAD prototype. The enclosure has not been printed or tested.

## Dimensions

- PCB outline: 100 × 83.5 mm
- PCB mounting holes: 92 × 75.5 mm apart
- Enclosure body: 110 × 93.5 mm
- Base thickness: 3 mm
- Wall thickness: 2 mm
- Wall height above the inner floor: 32 mm
- Lid thickness: 2 mm
- PCB posts: 8 mm above the inner floor

## Known limitations

- The heat-set insert holes need a test print before I print the whole enclosure.
- I still have to check the connector openings with the real plugs and cables.
- The imported models don’t show things like solder joints or bent cables, and the real parts can be a bit different.

## Documentation

The BOM and the journal are synchronized from [Half Life](https://halflife.hackclub.com/), so changes I make to them here can be overwritten.

I am making an effort to document my work in English, but my English is still limited. I use a AI to help explain the project and describe my progress.

## Third-party models

I use the imported PCB and component models only to check dimensions. I did not make them, and if any of them end up in this repository they keep their own licences.

## License

See [LICENSE](LICENSE). It does not cover the third-party models.

## Inspiration

Inspired by Hyperspace Pirate’s electromagnetic accelerator project.
