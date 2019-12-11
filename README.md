# cpe476
repo for mobile robotics cpe476

CPE-476 Tasks

Task 1: Description of the Mobile Robot, include documentation and reference to datasheets, images, assembly instructions, etc. 
  Reference to datasheets
  Romi32U4 Board 
  https://www.pololu.com/file/0J1258/romi-32u4-control-board-schematic-diagram.pdf
  https://www.pololu.com/file/0J1261/romi-32u4-control-board-pinout-power.pdf
  Romi Encoder 
  https://www.pololu.com/file/0J1208/romi-encoder-pair-kit-schematic-diagram.pdf
  https://www.pololu.com/file/0J1210/romi-encoder-dimension-diagram.pdf
  Wheel Motor
  https://www.pololu.com/file/0J822/mini-plastic-gearmotor-90-degree-dimension-diagram.pdf
 
Task 2: Motor and Encoder Testing - In this task, the team will perform basic tests for the motor (proper forward, backward, right and left motion), and encoder operations.
  For this task we ran the Encoder test and Motor test. Both tests ran fine.
  
Task 3: Wheel Calibration (fix systematic errors)- The goal of this task will be to move your robot using built-in commands for a distance  of 2 meters. Determine the trim values of the motor such that the robot travels in a straight line. 
  Our robot need to be calibrated a bit as the right motor was running about 2% faster than the left. Our robot was able to drive straight   after minimal calibration
  
Task 4: Unidirectional & Bidirectional Square Path Experiment - In this task the robot, follows a path comprising of four straight line segments and four pure rotations about the robot's center point, at the corners of the square. The robot's end position visualizes the dead-reckoning error.
  for this test we had the robot drive straight for a meter, then with trial and error determined the speed/time it would take in order   for   the robot to turn a perfect 90 degrees using speed of motorA = -speed of motorB. This worked for us and the robot made a perfect   square path. 
  
Task 5: PID Contol - Implement PID control to offset unknown tracking errors. Use supplied K values. You can modify them later. 
  for this test we ran the PID example found here https://gist.github.com/bradley219/5373998. With a few modifications it ran.
  
Task 6: Dead reckoning - Using the of motor encoder values, calculate the robot's position and pose for the motor basic test.
  for this test we used https://github.com/purwar2016/DeadReckoning-library and applied it to the motor test. with many modifications we   were able to program our Romi board.
Task 7: Interface IMU: Interface the IMU on the board to get acceleration and gyro values. Create a message including odometry and IMU values and transmit the message to the Host PC and log the data in Rviz.
  for this task we used https://github.com/pololu/romi-32u4-arduino-library. acceleration was fine. We did have issues with the gyro       values at first, but ended up replacing our board for other purposes. After this the gyro values were fine. 
Task 8:
Task 9: Setup your RPI: Use the raspberry pi 3+/4 to setup Raspbian + ROS (Kinetic/Medoldic) + OpenCV.
  for the OS on our RPI3 we installed Ubiquity's https://downloads.ubiquityrobotics.com/pi.html. This made the process very simple. We then expanded the memory, eneabled ssh, and made other changes to settings following along in class. 
  

