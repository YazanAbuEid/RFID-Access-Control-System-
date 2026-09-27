# EE — Biometric access-control kiosk

This directory contains the electrical/embedded work for the joint biometric access-control project. The shared backend repository is `mjdakkak/Biometric_Access_Control_System`.

## Layout

- `firmware/`: PlatformIO project for the Freenove ESP32-S3-WROOM camera board.
- `nextion/`: editable NX3224F028_011 display project and interface notes.
- `hardware/`: pin allocation and prototype power/wiring notes.
- `docs/`: setup, backend interface, test status, and outstanding integration work.

Open **`EE/firmware`** as the PlatformIO project, not the repository root. Create a private `firmware/src/secrets.h` from the example; never commit credentials or firmware binaries containing them.

The prototype is a **single-kiosk** system. Backend approval is not physical door-open confirmation. Fingerprint recovery integration and real hardware verification remain pending; lock output stays disabled until the physical circuit is verified.
