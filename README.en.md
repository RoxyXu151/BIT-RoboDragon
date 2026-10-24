# BIT-RoboDragon

[简体中文](README.md) | **English**

Arduino robot-car control code for the BIT RoboDragon challenge, including Bluetooth remote control, infrared line following, ultrasonic obstacle avoidance, and variant-specific actuator or servo control.

## Requirements

Arduino UNO, Arduino IDE, drivers, and a serial port. The servo variant needs the Servo library and matching hardware.

## Get the repository

```bash
git clone https://github.com/RoxyXu151/BIT-RoboDragon.git
cd BIT-RoboDragon
```

Private repositories require GitHub authentication. Relative paths and steps below start from this repository.

## Setup and entry point

Use the editor or reading tools described below; there is no shared command-line launch sequence.

## Configuration and preparation

Open bth_v2/bth_v2.ino or tulong/tulong.ino and select UNO and the correct port. leftPWM, infrared, and shoot pins differ between variants; wire against the selected sketch definitions and do not mix pin maps. Serial baud rate is 9600.

## Usage and outputs

Compile before uploading and test the selected program’s mode sequence. Remote commands F/B/L/R/S control forward, backward, left, right, and stop. A controls the base variant actuator and E the servo variant. Confirm C/D mode exits in the selected sketch.

## Repository map

- [bth_v2](bth_v2)
- [tulong](tulong)
- [Original detailed material](README.reference.md): historical design, screenshots, and notes are retained; use the checked setup guidance above where it differs.

## Verification and troubleshooting

Check direction and stopping with wheels off the ground before low-speed sensor, line-following, and obstacle tests. Close the serial monitor if it blocks uploads. No hardware automation tests are provided.

## Maintenance and contributions

Keep both READMEs in sync when functionality or usage changes. Report reproducible steps, environment versions, and sanitized logs. Describe the verification actually performed with each change.

## License and attribution

See [LICENSE](LICENSE) for repository terms. Third-party code, data, models, papers, and artwork retain their own licenses and attribution.
