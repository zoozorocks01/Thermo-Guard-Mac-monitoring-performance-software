# Thermo-Guard-Mac-monitoring-performance-software
Apple Silicon-first Mac monitoring app focused on thermals, performance, and transparency. Support for late- gen Intel chips will come later

# ThermoGuard

ThermoGuard is a macOS system monitor focused on thermals, performance, and transparency.

Built Apple Silicon first, ThermoGuard is designed to help you understand what your Mac is doing without pretending every reading is equally certain. The long-term goal is a monitor that can clearly distinguish between measured, inferred, and unavailable data, while also showing the cost of monitoring itself.

## Why ThermoGuard?

Most monitor apps focus on showing more numbers.

ThermoGuard is aiming for something a little different:

- **Trust first**  
  Readings should be honest about whether they are measured, inferred, experimental, or unavailable.

- **Transparency**  
  The app should make it clear where data comes from, how confident it is, and what it costs to collect.

- **Whole-machine context**  
  Thermals matter, but so do CPU load, memory pressure, disk state, process activity, and monitoring overhead.

- **Scalable complexity**  
  ThermoGuard should work as a lightweight menu bar tool, a standard dashboard, and eventually a deeper x-ray style diagnostic view.

## Current status

ThermoGuard is currently an active prototype.

### Working now

- Live dashboard
- Menu bar utility behavior
- Top Apps / process view
- Settings persistence
- Degree of Concern system
- Observer-impact view for ThermoGuard’s own overhead
- Capability profile view
- Experimental raw Apple Silicon sensor display

### In progress

- Exact CPU and GPU temperature support --> looks like it may have to be inferred
- Raw sensor interpretation and mapping
- Deeper capability handling across machine and backend types
- UI polish and richer diagnostic views

## Design direction

ThermoGuard is being built around a provider-based architecture so that safe fallback paths, experimental backends, and future platform-specific support can all fit the same model.

The goal is not just to show temperatures. The goal is to help users understand:

- what the machine is doing
- how trustworthy each reading is
- what the app itself costs to observe the system

## Current principles

- measured vs inferred vs unavailable should be explicit
- experimental features should stay honest
- monitoring overhead should be visible
- lightweight everyday use should come first
- deeper diagnostic views should be opt-in

## Roadmap

Near-term priorities include:

- refining Apple Silicon temperature interpretation
- improving exact-temperature backend strategy
- continuing UI polish
- expanding observer-impact reporting
- building richer raw-vs-inferred views

## Notes

ThermoGuard is under active development, and some experimental features may change as the telemetry model and backend strategy evolve.
