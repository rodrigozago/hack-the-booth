# Software Architecture

## Boot process

1. Linux boots and initializes audio/MIDI devices.
2. Hack the Booth startup service validates hardware presence.
3. UI launcher starts in kiosk-friendly mode.
4. Mixxx launches with predefined profile and mappings.

## Core components

- **Mixxx startup**: preconfigured startup profile and skin selection.
- **Controller mappings**: versioned mapping files for supported controllers.
- **Audio configuration**: ALSA/PipeWire profile for master/cue routing.
- **MIDI routing**: direct controller mapping with optional middleware layer.
- **UI launcher**: touchscreen-first launcher for performance and utilities.
- **Configuration system**: editable project config for devices and startup behavior.
- **Update system**: scripted update workflow with rollback guidance.

## Design principles

- Deterministic startup for live reliability
- Transparent configuration in plain-text files
- Reproducible setup on Raspberry Pi
- Safe fallback behavior when devices are missing
