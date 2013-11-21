Robot_Movement_Library
======================

Contains the code neccesary to move the robot's different motors, and move the robot in certain directions

Functions:

void initMotorTimer()- Initializes the timer on the robot

void leftMotorForward()- moves the left motor forward

void rightMotorForward()- moves the right motor forward

void leftMotorBackwards()- moves the left motor backwards

void rightMotorBackwards()- moves the right motor backwards

void moveRobotForward()- moves the robot forward

void moveRobotBackwards()- moves the robot backwards

void moveRobotSharpLeft()- makes the robot do a sharp turn left

void moveRobotSharpRight()- makes the robot do a sharp turn right

void moveRobotLeft()- makes the robot turn left

void moveRobotRight()- makes the robot turn right

void stopRobot()- stops the robot


Sample code:

void leftMotorForward() {
    
    TA0CCTL0 |= OUTMOD_5;
    _delay_cycles(10000);
    TA0CCR1 = 60;
    
}

This code makes the left motor go forward by setting the output mode to reset and setting the duty cycle
to sixty percent.
