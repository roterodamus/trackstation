# TrackStation

### Description
TrackStation is a lightweight, multi-platform/multi-architecture groove box written in C/C++. It is designed with game-pad controls and a page-structure navigation, featuring a simple yet powerful user interface. All essential functions (mixer, transport, system handling, etc.) are UI-optimized CLAP plugins supporting modulation and open-source community plugins. Similar to OpenElec with Kodi or Recalbox with EmulationStation, TrackStation is available as a standalone application or as a Just Enough Operating System (JEOS). It runs on Raspberry Pi, Chinese retro gaming handheld devices, and old laptops/computers, saving them from the dumpster.

### Notes
Godot, although primarily a game engine, is a good starting point for developing TrackStation due to its handling of game-pad input and user interface design. It also integrates well with C++ and can work with Tracktion Engine and JUCE. Tracktion Engine is the backbone of Tracktion Waveform DAW, and JUCE is a framework for audio application and plugin development.

*Currently, JUCE and the Tracktion Engine do not support CLAP plugins.*

**Consideration:** Does JUCE's GUI and gamepad support make Godot unnecessary?

### Name
Possible name candidates:
- TrackStation (high contender)
- MuseStation
- ..somethingStation
- NinTuneDo (instant cease and desist)

## Features

### Instruments
- **VA additive synth (Odin2):** [Odin2 GitHub](https://github.com/TheWaveWarden/odin2)
- **FM Synth (Dexed):** [Dexed](https://asb2m10.github.io/dexed/)
- **303 bass synth (Open303):** [Open303](https://github.com/RobinSchmidt/Open303) & [JC303](https://github.com/midilab/jc303)
- 8 voice Drum synth??
- MIDI out (note, cc, pc)
- Other Synths?
- Drum sample player
- Recorder
  - Looper (tempo detection???)
  - Re-sampling
  - Sample manipulation
    - Time stretching
    - F, rev, ping-pong, fade-in-out
    - Key mode (poly)
    - Slice mode
      - Peak detection
      - Equal divided
      - Lazy chop
    - Stems splitter?????

### Sequencer
- Song mode (free clip placement)
- Clip-based (resizable in song mode)
- Audio tracks
- MIDI out (external synth)
- Automation
  - LFO/modulation matrix (extensive modulation)
  - MIDI modulation
- MIDI tracks
  - List mode (tracker style) (step-fx?)
  - Piano grid (chord mode???)
  - Step-sequencer (P-Locks?)
  - x0x-style sequencers
  - Alternative sequencers?

### Mixer
- Pan 
- Minimum 8 tracks (preferably more)
- Bus tracks
  - Effects
    - Reverb, Delay 
    - EQ, filter
    - Chorus/flanger, phaser, stereo-fx
    - Compressor/expander (sidechain)
    - Distortion, Bitcrusher, etc.
    - Up to 4 per track
    - LFO control
    - Guitar/bass effects (amp emulation)

### System
- Game-pad based navigation 
  - Minimal: D-pad + 10 buttons (PS1 controller)
  - Preferred: D-pad + 12 buttons and 2 analog sticks (Xbox/PS2 and up controller)
- Random name generator
- Full keyboard support for navigation, naming & number input (not necessary)
- Mouse support???
- 2 display modes: scalable low-def (640x480) & high-def (1280x720 or 1920x1080???)
- MIDI support (MIDI 2.0???)
- MIDI learn
- MPE???
- Audio multi-in-out???
- Networking?
  - Web-server file management
  - Ableton Link: [Ableton Link GitHub](https://github.com/Ableton/link)
  - RTP-MIDI??? [RTP-MIDI GitHub](https://github.com/davidmoreno/rtpmidid)
- BLE-MIDI???

## Other Links
- Tracktion Engine: [Tracktion Engine GitHub](https://github.com/Tracktion/tracktion_engine/)
- JUCE: [JUCE](https://juce.com/)
- Godot: [Godot Documentation](https://docs.godotengine.org/en/stable/index.html) & [Godot FAQ](https://docs.godotengine.org/en/stable/about/faq.html#is-it-possible-to-use-godot-to-create-non-game-applications)
- CLAP: [CLAP](https://cleveraudio.org/)
- Synthesis Tool Kit: [Synthesis Tool Kit GitHub](https://github.com/thestk)
- MI Open-source modules (IC): [Mutable Instruments Documentation](https://pichenettes.github.io/mutable-instruments-documentation/)
- USB bootable operating system: [Just Enough Operating System](https://en.wikipedia.org/wiki/Just_enough_operating_system)
- Possible graphics libraries: [Raylib](https://www.raylib.com/)
- FFT library: [FFTW](https://www.fftw.org/)
- Fast CLI MPEG play & dec lib: [MPG123](https://www.mpg123.de/)
- Stems splitter: [Spleeter GitHub](https://github.com/deezer/spleeter)

## Inspiration

### Dirtywave M8
[Dirtywave M8](https://dirtywave.com/)
An excellent minimal user interface and workflow with just 8 buttons, creating a powerful little device.

### OpenELEC, Lakka, Batocera, Recalbox, RetroPie (EmulationStation)
USB bootable single-purpose operating systems for playing retro games or creating a home theater system, compatible with various hardware.

### Zynthian
[Zynthian](https://zynthian.org/)
An open-source synthesizer project for Raspberry Pi SBCs, serving as a hardware LV2 plugin host.

### Akai MPC/Force
[Akai MPC Series](https://www.akaipro.com/products/mpc-series)
Akai's DAW in a box with new MPCs and the Force, running custom software on a custom Linux distribution and hardware (SoC: RK3288, RAM: 2GB, ROM: 8GB).

### LMN-3
[LMN-3 GitHub](https://github.com/FundamentalFrequency)
A similar open-source project inspired by the Teenage Engineering OP-1, written in C++ with JUCE and the Tracktion Engine.
```
