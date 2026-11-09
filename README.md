How to Use Features
1. Waypoints & Actions on Arrival
Waypoints are goal points on the mat. Your robot turns toward a waypoint, drives straight to it, and turns to match the waypoint's heading angle.

Drag Target: Drag the center dot to move the location; drag the orange handle to rotate the target angle.
Actions on Arrival: Click + Add... on any waypoint card to program actions when the robot reaches that spot—such as pausing, spinning attachment motors, or playing a sound.
Optimize Path: Click the green Optimize path button to automatically delete unnecessary intermediate points along straight lines!
2. Launch Snapping & Wall Positioning
In FLL, placing your robot squarely against the border wall is key for repeatable runs.

Snap SW / SE: Instantly snaps Waypoint 1 into the official Southwest or Southeast launch arcs.
Wall Dropdown: Select Bottom, Top, Left, or Right to force Waypoint 1 flush against a wall taking your robot's exact chassis dimensions into account.
Gap Offset: Add a small gap (e.g. 5 mm) if your attachment extends past your chassis frame.
3. BIOGLOW™ Mission Interactive Scorer
Track points for the official 2026–27 BIOGLOW™ challenge right inside the tool!

Missions Tab: Expand mission cards to check off completed objectives and calculate your score automatically.
Canvas Markers: Click numbered mission dots on the map to open the corresponding mission details card instantly.
Move Markers: Check "Move markers" to drag mission points so they match your custom mat alignment.
4. Exporting Gyro-Corrected Code
Path Studio generates code that uses your hub's IMU Gyro sensor to keep the robot moving perfectly straight and turning accurately on the physical mat.

Select your environment: Pybricks Python, Pybricks Blocks, SPIKE Prime Python, EV3 MicroPython, or Human Driver Steps.
Click Copy Code and paste it straight into your robotics software!
Step-by-Step Robot Physical Tuning Guide
Easy instructions for middle school students to calibrate their real robot to match the screen!

Why does my physical robot not move like the screen?
LEGO plastic wheels squish slightly under weight, and wheel axle spacing can differ by a few millimeters. Calibration fixes distance and turning errors so your robot drives on the mat exactly like it does in the simulator!

A
Calibrating Driving Distance (Wheel Diameter)
Fixes over-shooting or stopping short
STEP 1
In the Tuning tab, click 50 cm Straight Test Path.

STEP 2
Set your robot up against the back wall on your real FLL mat. Place a ruler or tape measure along the edge of your robot.

STEP 3
Export and run the code. Measure how far the robot actually moved on the mat with your ruler (e.g. 48.5 cm instead of 50 cm).

STEP 4
Under Distance Calibration on the Tuning tab, enter 50 in Commanded Distance and 48.5 in Actual Measured Distance, then click Adjust Wheel Diameter.

Result: Your Wheel Diameter parameter automatically updates to eliminate distance errors!
B
Calibrating Pivot Turns (Track Width / Autotune)
Fixes under-turning or over-spinning
STEP 1
In the Tuning tab, click 180° Spin Test.

STEP 2
Align your robot precisely parallel to a grid line on your mat.

STEP 3
Export and run the code. Watch where the robot stops spinning. Did it complete a half turn (facing the opposite way), or did it stop early / turn too far?

STEP 4
Under Turn Calibration (Autotune), enter 180 in Target Angle and your actual measured turn angle (e.g. 190°) in Actual Measured Turn Angle, then click Adjust Track Width.

Result: Your Axle Track Width parameter automatically re-calculates for perfect turns!
