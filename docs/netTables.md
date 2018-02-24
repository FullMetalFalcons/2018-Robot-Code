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
