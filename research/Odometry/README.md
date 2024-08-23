### Reading Odometry

Odometry is the process of measuring and tracking the distance traveled by a robot. It is based on the coordinated operation of all the robot's sensors, which help determine its position and orientation in space.

1. **Gyro Sensor**: The gyroscope measures the robot's rotation angle. This sensor allows you to determine a change in the direction of movement and calculate the current rotation angle, which is important for maintaining the correct course.

2. **Encoders**: Encoders are built into the robot's motors and measure the number of revolutions made by the motor shaft. Knowing the number of revolutions and the diameter of the wheel, you can calculate how far the robot has traveled. This is done using formulas that relate the number of encoder pulses to physical distance.

3. **Color Sensor**: The color sensor is used to detect markers on the floor, which signal the robot to reset the odometry. This allows the robot to reset its data and start over, which is important for maintaining accuracy, especially when navigating complex paths.

### Local Odometry

To improve navigation accuracy, the robot divides the map into four zones. Each zone represents a section of the path on which the robot takes its odometry measurements. This is done to avoid the accumulation of errors when measuring distances and turning angles.

1. **Dividing the Map into Zones**: The robot's route map is divided into four zones, each containing certain turning points. This allows the robot to more easily track its position, since each zone is a relatively small section of space.

2. **Reading Odometry in Each Zone**: Within each zone, the robot measures its position and turning angle using a gyroscope and encoders. This data is used to build a map and plan its movement.

3. **Odometry Reset on Turns**: Each time the robot turns, it resets its odometry and gyroscope values ​​using the data from the two lines it crosses using the color sensor. The robot reads the position relative to the first and second lines and calculates the difference between them using mathematical formulas. These calculations allow the robot to accurately determine the angle of the turn and adjust its gyroscope and odometry readings, ensuring that it continues to move along the intended path.

4. **Waypoint Recording**: As the robot moves through each zone, and especially when turning, it records the coordinates of the points. A total of 16 checkpoints are generated after passing all the zones. These points allow the robot to adjust its trajectory and ensure that it follows the intended route accurately. ### Formulas for Calculations

The following formula is used to calculate the distance traveled by the robot:

- **15.43 cm per revolution**: This value was calculated based on the data about the wheel diameter and the number of revolutions made by the encoders. The formula for calculation is as follows:

**Circumference** = π × Wheel Diameter

Where π ≈ 3.14, and the wheel diameter is measured in centimeters.

Knowing the circumference of the wheel and the number of revolutions made by the encoder, we can calculate the distance traveled:

**Distance Traveled** = Number of Revolutions × Circumference

This formula helps the robot determine how much it has traveled based on the encoder data.

### Application of Odometry in Robot

These approaches allow the robot to accurately follow a given trajectory, adjust its movement based on sensor readings, and return to predetermined points. When combined with other sensors and features such as color-coded odometry reset, the robot can perform complex spatial navigation tasks reliably and accurately.