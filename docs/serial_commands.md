# Robot Arm Serial Commands

Use Arduino Serial Monitor at 9600 baud.
Set line ending to Newline or Both NL & CR.

## Basic commands

| Command | Meaning |
|---|---|
| HELP | Show commands |
| STATUS | Show current angles |
| HOME | Move arm to home position |
| STOP | Stop/detach servos |
| OPEN | Open gripper |
| CLOSE | Close gripper |

## Servo commands

| Command example | Meaning |
|---|---|
| BASE 90 | Move base to 90 degrees |
| SHOULDER 100 | Move shoulder to 100 degrees |
| ELBOW 80 | Move elbow to 80 degrees |
| GRIPPER 40 | Move gripper to 40 degrees |

## Recommended angle limits

| Joint | Safe range |
|---|---|
| Base | 0 to 180 |
| Shoulder | 20 to 160 |
| Elbow | 0 to 180 |
| Gripper | 10 to 110 |

## Troubleshooting

If the servo shakes, use a stronger external 5V power supply.
If movement direction is wrong, reverse the servo horn position or adjust angles in code.
If the arm hits the frame, reduce the angle range before testing again.
