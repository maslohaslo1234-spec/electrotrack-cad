# Electrotrack CAD

<img width="1271" height="811" alt="assembly" src="https://github.com/user-attachments/assets/2426da56-25cd-49e5-9ec3-12dea68f4e0b" />


This repository has the mechanical design of my Electrotrack project: the enclosure for the PCB and the parts of the circular track. I modelled everything in Onshape during Week 2 of Hack Club Half Life.

The electronics (schematic, PCB and firmware) are in a separate repository:

[Electrotrack electronics](https://github.com/maslohaslo1234-spec/electrotrack)

## What is Electrotrack?

Electrotrack is an experimental electromagnetic ball accelerator that I am building. The goal is to accelerate a metal ball around a circular track using electromagnetic coils.

The project combines a custom PCB, an ESP32 microcontroller, IR sensors, electromagnetic coils, and 3D-printed mechanical parts.

This repository contains the mechanical design of the project, including the PCB enclosure, track segments, coil formers, and sensor mounts. The electronics are documented in a separate repository.

## How is it supposed to work?

The idea is to place electromagnetic coils along a circular track. IR sensors will detect when the ball approaches each coil, and the ESP32 will use this information to control when the coils are activated.

When a coil is energized at the right moment, its magnetic field attracts the ball and helps accelerate it. By activating the coils in sequence, the system is intended to keep the ball moving around the track.

The 3D-printed parts are important because they hold the coils and sensors in position, guide the ball, and provide mounting points for the electronics.

This is still a prototype, so the complete system has not been tested yet.

## Why am I building it?

I was inspired by Hyperspace Pirate's electromagnetic accelerator project and wanted to try designing my own version.

I am interested in electronics and 3D printing, and this project gives me an opportunity to combine them. I want to learn more about electromagnetic acceleration, PCB design, microcontroller programming, and designing mechanical parts that work together.

During this stage, I am focusing on the mechanical design. My goal is to create parts that can be 3D printed, assembled, and tested with the real electronics.

## Firmware Development

I am currently working on the firmware for the ESP32, which will read data from the IR sensors and control the electromagnetic coils.

Once the firmware is ready, I plan to upload it to my [Electrotrack electronics repository](https://github.com/maslohaslo1234-spec/electrotrack), which I created during Week 1.

The firmware is still under development and has not been tested with the complete system yet.

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

## Onshape CAD Model

The complete CAD model is available in Onshape:

[View Electrotrack CAD in Onshape](https://cad.onshape.com/documents/5df0b1e35f7d42ba30c57c01/w/6c10c4b5d57773fbd70dbcb3/e/2c0a8ce66aa1fa0771c34378)

The document contains the PCB enclosure, track components, and assembly.


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

I am making an effort to document my work in English, but my English is still limited. I use AI tools to help translate and improve the English in my project documentation.

## Third-party models

I use the imported PCB and component models only to check dimensions. I did not make them, and if any of them end up in this repository they keep their own licences.

## License

See [LICENSE](LICENSE). It does not cover the third-party models.

## Inspiration

Inspired by Hyperspace Pirate’s electromagnetic accelerator project.
