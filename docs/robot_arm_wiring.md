# Robot Arm Wiring Guide

This file explains the basic wiring for a small educational Arduino robot arm.

## Parts

- Arduino UNO or Nano
- 4 servo motors
- External 5V power supply for servos
- Jumper wires
- Small robot arm frame

## Servo pin map

| Joint | Arduino Pin |
|---|---|
| Base | D3 |
| Shoulder | D5 |
| Elbow | D6 |
| Gripper | D9 |

## Power safety

Do not power all servos directly from the Arduino 5V pin.
Use a separate 5V supply for servos.
Connect the servo power supply GND with Arduino GND.

## Testing steps

1. Connect only one servo first.
2. Upload a simple servo test sketch.
3. Confirm movement is smooth.
4. Connect the remaining servos one by one.
5. Test every joint before attaching the full arm load.

## Notes

Keep fingers away from moving joints while testing.
Set angle limits in code before running the full arm.
