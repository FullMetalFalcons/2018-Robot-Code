# Network Table Variables

This file documents all the variables being sent through NT from the robot to the dashboard and back.

## Dashboard --> Robot

Tele-Op Constants:
- `outtakeSpeed` - speed the shooter should shoot at (0-1)
- `intakeSpeed` - speed the shooter should intake at (0-1)
- `climbCurLim` - the current limit for the climber in Amps
- `reverseClimber` - reverse climber for unwinding of rope; in match should be False

Autonomous Mode Constants:
- `autoWait_s` - time the robot should wait before beginning auto in seconds; default should be 0
- `autoMode` - autonomous mode the robot should run; see below for list autonomous modes (0-11)
- `startSide` - the side the robot is starting; see below for list of start sides

Drive Velocity PID Constants:
- `leftDrive_P` - P constant for the left drive
- `leftDrive_I ` - I constant for the left drive
- `leftDrive_D` - D constant for the left drive
- `leftDrive_F ` - F constant for the left drive
- `rightDrive_P` - P constant for the right drive
- `rightDrive_I ` - I constant for the right drive
- `rightDrive_D` - D constant for the right drive
- `rightDrive_F ` - F constant for the right drive

Autonomous Position PID Constant:
- `leftPos_P` - P constant for left position
- `leftPos_I` - I constant for left position
- `leftPos_D` - D constant for left position
- `rightPos_P` - P constant for right position
- `rightPos_I` - I constant for right position
- `rightPos_D` - D constant for right position

Ramping Constants:
- `turnS1` - Top turning speed (units: ticks/100ms, should be 1 - 4200)
- `turnD2` - Angle from target at which to ramp down to S2 (degrees)
- `turnS2` - Bottom ramp speed (units: ticks/100ms, should be 1 - 4200)
- `driveS1` - Top drive forward speed (units: ticks/100ms, should be 1 - 4200)
- `driveD2` - Distance from target at which to ramp down to S2 (degrees)
- `driveS2` - Middle ramp speed (units: ticks/100ms, should be 1 - 4200)
- `driveD3` - Distance from target at which to ramp down to S3 (degrees)
- `driveS3` - Bottom ramp speed (units: ticks/100ms, should be 1 - 4200)

### Autonomous Modes
ID | Name
---|---
0 | Do nothing
1 | Cross baseline short
2 | Cross baseline long
3 | Hot from middle
4 | If hot 2 cubes, else 1 cube
5 | If hot 1 cube, else 1 cube
6 | Exchange from middle
7 | Forward to switch, score if hot
8 | Exchange from outside
9 | If hot 2 cubes, else baseline
10 | If hot 3 cubes, else baseline
11 | Exchange and hot switch

### Start Position
ID | Name
---|---
0 | right
1 | left
