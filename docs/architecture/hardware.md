# Hardware Architecture

## Core system

- Raspberry Pi as central compute unit
- Powered USB hub for controller/interface expansion
- USB DJ controller for transport, jogs, mixer controls, and performance pads
- USB audio interface for stable low-latency output
- Optional touchscreen for local UI and configuration

## Subsystems

### Raspberry Pi integration
- Boots Linux and launches the Hack the Booth startup flow.
- Hosts Mixxx and middleware for audio/MIDI routing.

### Power supply
- Dedicated Pi power supply sized for stable current delivery.
- Separate powered USB hub to avoid brownouts from controller + audio load.

### USB hub topology
- Pi USB root -> powered hub -> controller + audio + optional peripherals.
- Keep controller and audio interface on direct hub ports (no chained hubs).

### Audio interfaces
- Prefer class-compliant USB audio interfaces.
- Route master output and headphone cue through ALSA/PipeWire profiles.

### MIDI communication
- USB MIDI from controller to Mixxx mapping layer.
- Optional virtual MIDI bridge for diagnostics and remapping.

### Touchscreen support
- 7" touchscreen optional for browsing, setup, and utility screens.
- Use touch-friendly launcher for booth operations.

### 3D printed parts
- Mounting brackets for Pi, hub, audio interface, and touchscreen.
- Cable guides and strain relief to improve reliability.

## Assembly (high-level)

1. Install printed mounts in enclosure or frame.
2. Secure Pi and powered hub.
3. Mount audio interface and route short USB cables.
4. Attach touchscreen and cable strain relief.
5. Power on and validate USB/audio/MIDI detection.
