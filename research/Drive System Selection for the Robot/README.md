## Research: Front vs Rear Wheel Drive for a Robot

### Research Objective
To examine the key advantages and disadvantages of front and rear wheel drive in robotics, aiming to select the optimal option for enhancing the stability, accuracy, and maneuverability of our robot. This research also analyzes the design constraints and operational features of using LEGO construction and justifies the choice of rear wheel drive for our project.

---

### Key Aspects of Front vs Rear Wheel Drive Comparison

| Criterion                          | Front Wheel Drive                                                                                                                                | Rear Wheel Drive                                                                                                                                      |
|-----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stability and Traction**      | Front wheel drive can be stable at low speeds and on smooth surfaces but loses traction at high speeds due to weight transfer. | Rear wheel drive maintains traction and provides stable acceleration and braking, especially with sufficient weight on the rear axle.          |
| **Maneuverability on Turns**    | Front wheel drive is more predictable at low speeds, can correct trajectory due to steering with front wheels, but prone to understeer at high speeds. | Rear wheel drive reduces understeer during maneuvering at speed, improving control and reducing deviation from the course, especially during dynamic movement. |
| **Traction**                  | Can handle inclines better due to more weight on the front wheels, but loses traction on slippery surfaces.             | Provides even weight distribution, improving traction on different surfaces and during acceleration on a flat surface.         |
| **Weight Distribution**        | Requires shifting the center of gravity closer to the front axle to optimally utilize the front wheels as both pulling and steering elements.             | Shifting weight towards the rear improves traction of the rear driving wheels, reduces slippage, and makes it easier to adjust optimal stability and handling. |
| **Design Simplicity**      | Front wheel drive with steering front wheels requires more components and complicates the design, especially using LEGO parts.            | Separation of traction and steering functions simplifies the design, as drives are located on the rear axle and steering mechanisms are on the front, reducing wear and tear. |

---

### Additional Criteria and Design Features

| Criterion                         | Front Wheel Drive                                                                                             | Rear Wheel Drive                                                                                                         |
|----------------------------------|------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| **Steering Mechanism**             | Front wheels perform two functions: steering and traction, leading to increased wear and tear.    | Steering and driving wheels are separated, simplifying design and reducing wear on parts, especially when working on small radii. |
| **Weight Distribution and Balance** | Requires precise weight shifting towards the front wheels, which is difficult to achieve when assembling from LEGO parts.            | Placing drive components on the rear axle improves balance and traction, reducing slippage.         |
| **Impact on Frame Design**  | The need to mount motors and steering mechanisms at the front complicates balancing and makes the design bulky.            | Rear drive allows for compact component placement at the rear, simplifying setup and increasing stability while reducing centering. |
| **Reliability**                   | May require more complex control to avoid slipping and deviations from the course at high speeds.    | More reliable at high speed and sharp turns, as it minimizes understeer and improves predictable robot behavior.  |

---

### Analysis: Pros and Cons of Front vs Rear Wheel Drive for Our Project

1. **Stability**: For a robot that needs to perform complex maneuvers, rear wheel drive is more preferable. Rear wheel drive is stable at high speed, reduces the likelihood of skidding and slipping, especially if the center of gravity is shifted towards the rear. This aspect is essential for stable trajectory passage and maneuvering without deviations from the course.

2. **Balancing and Weight**: LEGO parts have fixed dimensions and limited options for optimizing weight distribution. Placing motors and drive elements on the rear axle improves robot balance, as the center of gravity shifts closer to the rear wheels, providing good traction on turns and reducing slippage.

3. **Design Constraints**: Front wheel drive, requiring a load on the front axle, complicates the design, as the load on the front wheels leads to rapid component wear, increases energy consumption, and creates difficulties with balancing. In the case of the LEGO system, which has limited possibilities for customization and precise adjustment, rear wheel drive is optimal because it requires less effort during turns and reduces wear on parts.

---

### Tested Front Wheel Drive Assembly

During development, we initially assembled a test model with **front wheel drive** to assess its performance in real-world conditions. However, after conducting a series of tests, we concluded that front wheel drive did not meet our expectations for the following reasons:

1. **Center of Gravity**: In the front-wheel drive model, the center of gravity was significantly higher than in the rear-wheel drive robot. This was created because all the load was concentrated on the front axle, where the motors and wheels were located. This weight distribution reduced traction with the surface and impaired stability, especially during maneuvering.
2. **Motor and Wheel Operation**: In the front-wheel drive model, the front wheels performed two functions: they were both steering and driving. That is, the motors forced the front wheels to not only control movement but also pull the robot along the surface. While the rear wheels simply served as a support and did not have a significant load, except for supporting the robot in an upright position. This distribution of functions increased the load on the motors and caused accelerated wear and tear of components, which also negatively affected the durability of the design.

3. **Balancing Problems**: Given the limited capabilities of LEGO in weight distribution, front-wheel drive required additional weight on the front axle, which created additional difficulties in balancing the robot.

Based on these factors, we decided to abandon front wheel drive and choose **rear wheel drive**, which provided better stability, control, and energy efficiency for performing our robot's tasks.

<p align="center">
  <img src="../img/front wheel drive.jpg" width="40%" height="700px" style="margin-right: 10px;" />
  <img src="../img/front wheel drive2.jpg" width="40%" height="700px" />

</p>

---

### Final Justification: Choosing Rear Wheel Drive

Having considered all the features and requirements, we chose **rear wheel drive** for the implementation of our robot. This decision is based on the following advantages:

1. **Stability and Stability During Maneuvers**: Rear wheel drive provides reliable traction with the surface, which is especially important for moving along the trajectory and performing parking maneuvers. This allows the robot to confidently make turns and reduces deviations from the trajectory.

2. **Optimal Weight Distribution**: Placing the motor block on the rear axle improves balance and traction. This reduces the likelihood of wheel slippage, and the rear axle receives the optimal weight distribution necessary for stable and predictable movement.

3. **Simplified Design**: Rear wheel drive frees the front wheels from traction effort, which reduces the load on the steering mechanisms and simplifies their design. In the context of using LEGO parts, this significantly reduces wear and tear and increases reliability.

4. **Reliability and Stability in the Long Term**: Using rear wheel drive allows the robot to better handle acceleration, braking, and sharp turns without excessive load on the front wheels and steering mechanism.

**Conclusion**: Rear wheel drive meets our goals of improving stability, maneuverability, and energy efficiency, making it the optimal solution for this project.