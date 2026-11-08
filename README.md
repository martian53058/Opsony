# Opsony — Sony ULT WEAR Head Tracker for OnePlus 13

Source project for OnePlus 13 PJZ110 / ColorOS 17 / Android API 37.

This repository builds:
- the privileged Android HID Host helper app;
- the KernelSU module and its system permission/configuration files;
- a reproducible GitHub Actions build artifact.

The app relies on Android's existing Dynamic Sensor HAL to parse Sony Android Head Tracker HID reports and register `android.sensor.head_tracker` (type 37). It does not implement a second HID parser or fabricate motion data.

**Build status:** source and CI pipeline are being initialized. A successful build verifies compilation and packaging only; real PJZ110 Bluetooth HID, SensorService, and Spatializer behavior still require device validation.

See `README_CN.md` for architecture, setup, installation, and limitations.
