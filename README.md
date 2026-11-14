# RR OBD

A minimal, read-only diagnostics web app for the Range Rover Sport L494 3.0 diesel. It uses a Bluetooth Low Energy OBD adapter (tested target: vLinker MC+).

**Live app:** https://ihaseeburrehman.github.io/rr-obd/

## What it does
- **Live data:** RPM, coolant, fuel level, and DPF regen status, soot trigger % and the averages between regens (standard OBD PID 8B)
- **Faults:** shows only codes the car marks as *failed* or *confirmed* (engine and gearbox)
- **Custom read request:** send read-only requests (AT, 01–0A, 19, 22) to find manufacturer-specific values such as soot in grams

## Use it
1. Plug in the adapter and switch the ignition on.
2. Close any other OBD app (the adapter takes one connection at a time).
3. Open the app in **Chrome or Edge** (Mac, Windows, Android), or in the **Bluefy** browser on iPhone. Safari has no Web Bluetooth.
4. Tap **Connect** and pick the vLinker.

## Safety
This app is **read-only by design**. Write, routine and security requests are blocked in code. Use at your own risk; it is not affiliated with Jaguar Land Rover.

## License
MIT
