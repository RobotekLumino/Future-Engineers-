### Comparison of Polar and Cartesian Coordinate Systems for Competitions

#### Cartesian (normal) coordinate system

**Description:**
- **Simplicity and intuitiveness:** The Cartesian coordinate system represents the position of a point through two coordinates \(x\) and \(y\), which simplifies the control of the robot's movement.
- **Ease of calculations:** Rectilinear movements are easier to describe and calculate using the Cartesian system. Changes in the \(x\) and \(y\) coordinates directly reflect horizontal and vertical movements.
- **Integration with odometry:** Odometry in the Cartesian system is more intuitive, since the robot's movement on the plane is described by changing the values of \(x\) and \(y\).

#### Polar coordinate system

**Description:**
- **Compactness:** The polar system describes the position of a point in terms of radius(r) (distance from the center) and angle (theta) (angle relative to the axis), which is convenient for circular movements and rotations.
- **Convenience for rotations:** The robot's task is related to rotations or manipulation around a fixed point, the polar system can be more useful. (if you use the global coordinate system)

**Disadvantages:**
- **The difficulty of controlling rectilinear movements:** For most tasks related to linear movements, the polar system requires constant coordinate transformation, which complicates control.
- **Difficulties with integration into odometry systems:** The polar system is poorly suited for most odometric tasks, where a direct relationship between displacement and coordinate change is important.

### Why Do We Choose a Cartesian System for Local Odometry

1. **Converting polar coordinates to Cartesian coordinates:**
   - **No need for a polar system:** In our project, we would convert polar coordinates to Cartesian coordinates to work with odometry.
   - **Simplification of calculations:** Using a Cartesian system eliminates the need for constant transformations between coordinate systems, which simplifies programming and reduces the likelihood of errors.

2. **Optimization for local odometry:**
- **Ease of motion control:** Local odometry in the Cartesian system allows you to more accurately and intuitively control the movement of the robot along the trajectory, especially in areas with straight lines and simple maneuvers.
   - **Accuracy of calculations:** The Cartesian coordinate system makes it easier to track and adjust the robot's position in real time, which is important for accurate performance of tasks at competitions.
   - **Direct interaction with sensors:** Encoders and gyroscopes used for odometry work more efficiently in a Cartesian system, where changes in linear distance and angular displacement are easier to associate with the movement of the robot.

3. **Easy to use:**
   - **Fewer difficulties:** Using a Cartesian system reduces the complexity of robot control and simplifies software development, which is especially important in conditions of limited time at competitions.
   - **Increased reliability:** The Cartesian system makes control more predictable, which minimizes the risk of errors when moving the robot.

### The result

For tasks of local odometry and control of robot movement in competitions, the Cartesian coordinate system is a more appropriate choice. It simplifies calculations, makes control more intuitive and reduces the need for additional transformations, which increases the overall efficiency and accuracy of the robot. Polar coordinates can be used temporarily, but eventually they will be converted to Cartesian coordinates to ensure better integration with existing control and odometry systems.