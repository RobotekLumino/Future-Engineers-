# <div align="center"> Motor Selection</div> 
To compete in the World Robot Olympiad (WRO) in the Future Engineers category, we chose the LEGO Mindstorms EV3 Medium Motor. Let's take a closer look at the design features and benefits of a mid-motor, and explain why it is the optimal choice for this competition.
###  Brief description of motors
<div align="center">
<table>
<tr ><th colspan="3">NXT motor</th></tr>
<tr align="center">
<td><img src="./img/nxt.jpg" alt="NXT" align=center /></td>
<th>This motor is specific to the NXT set (2006). Includes a rotation encoder, returning to the NXT the position of the shaft with 1° resolution. Because of the special connector of this motor (non-standard phone plug type), a cable adapter is required to drive this motor with regular 9V sources. Not recommended for use with a RCX which can't deliver the high current that this motor can consume. Slow rotation speed, minimizing the need of external gear train.</th>
</tr>
</table>
<table>
<tr ><th colspan="3">EV3 Large motor</th></tr>
<tr align="center">
<td><img src="./img/ev3l.jpg" alt="ev3" align=center /></td>
<th>This motor is very similar to NXT motor, but with slightly better fixing capability (compatible with Technic frames, holes aligned with hub). Its efficiency seems slightly lower.</th>
</tr>
</table>
<table>
<tr ><th colspan="3">EV3 Medium motor</th></tr>
<tr align="center">
<td><img src="./img/ev3m.jpg" alt="ev3" align=center /></td>
<th>This motor is one of the highlights of EV3 set compared to NXT one: a motor of reduced size and classical front axle hub. Reduced size comes with reduced power, similar to PF medium motor (but being more down-geared, it is slower and delivers more torque).</th>
</tr>
</table>
</div>

### Rear-Drive DC Motor
- When selecting a DC motor among commonly available options in the market, considering factors such as weight, rotational speed, and torque, we have identified the following four suitable DC motors.
- Among them, the three types of motors, JGA25, have different model numbers but share a similar physical appearance, and their differences are as follows.
<div align="center"><table>
<tr ><th colspan="5">DC Motor Comparison</th></tr>
<tr align="center">
<th rowspan="2" >Model</th>
<th >JGA25 370</th>
<th >JGA25 370</th>
<th >JGA25 371</th>
<th >JGA16-050</th>
</tr>
<tr align="center">
<td ><img src="./img/JGA25-370_1360RPM.JPG" width = "150" alt="JGA25-370_1360RPM" /></td>
<td ><img src="./img/JGA25-370_620RPM.JPG" width = "150" alt="JGA25-370_620RPM" /></td>
<td ><img src="./img/JGA25-371_1_34.JPG" width = "100" alt="JGA25-371M" /></td>
<td ><img src="./img/JGA16-050.png" width = "150" alt="JGA16-050" /></td>
</tr>
<tr align="center">
<td >Speed</td>
<td >1360rpm</td>
<td >620rpm</td>
<td >294rpm</td>
<td >220rpm</td>
</tr>
<tr align="center"><td>Torque</td><td>4.27kg.cm</td><td>9.15kg.cm</td><td>5.2kg.cm</td><td>1.15kgcm</td></tr><tr align="center">
<td>Power</td><td>5.4W</td><td>5.4W</td><td>4.2W</td><td>0.33W</td>
</tr>
</table>
</div>  

- After conducting experimental research, we found that choosing the high-speed 1630rpm JGA-370 motor resulted in lower torque, making it difficult for the vehicle to move effectively. On the other hand, opting for the high-torque JGA-371 motor led to an excessively low rotational speed, which did not meet the requirements for the vehicle's operation.
- __Therefore, based on these findings, we ultimately selected the 620rpm JGA-370 motor as the rear-wheel drive DC motor for the vehicle. This choice strikes a balance between rotational speed and torque, providing the necessary performance for the vehicle's propulsion.__  

### Motor Drive Controller
- When testing the operation of the motor, simply providing power does not effectively control the movement of the GA25-370 motor, making it impossible to adjust the speed. Therefore, we need to install a motor controller to regulate the speed of the DC gear motor. Currently, there are two options available in the market: the L293D chip and the L298N module. To reduce weight, we __chose the smaller L293D chip.__   
- __Its compact size allows us to install more sensors, thereby saving space, reducing weight, and increasing the maneuverability of the vehicle.__


<div align="center">
<table>
<tr><th colspan="3">Motor Control Comparison</th></tr>
<tr align="center" >
<th rowspan="2">Model</th>
<th>L293D</th>
<th>L298N</th>
</tr>
<tr align="center">
<td> <img src="./img/l293d.png" width = "300"  alt="l293d" align=center /></td>
<td ><img src="./img/L298N.png" width = "300"  alt="l298n" align=center /></td>
</tr>
<tr align="center">
<td>Occupied Area(mm)</td>
<td>29.5x8</td>
<td>43.5x43.5</td>
</tr>
<tr align="center">
<td>Output Voltage</td>
<td>4.5V to 36V</td>
<td>5V to 46V</td>
</tr>
<tr align="center">
<td>Rated Power </td>
<td>5W</td>
<td>10W</td>
</tr>
</table>
</div>

# <div align="center">![HOME](../../other/img/Home.png)[Return Home](../../)</div>  
