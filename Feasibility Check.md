# Initial Check

| Categories                                                                   | CD1 (ramp/course) | CD2 (belt bench) | CD3 (hand crank) |
| ---------------------------------------------------------------------------- | ----------------- | ---------------- | ---------------- |
| Tabletop fit 500×250 mm                                                      | Fail              |                  |                  |
| Turn geometry: (i) left/right and (ii) front/rear travel different distances | Pass              |                  |                  |
| Full-time vs part-time 4WD in a turn                                         | Pass              |                  |                  |
| D3 locked axle in a turn                                                     | Pass              |                  |                  |
| Input ≤ 2.5 N·m                                                              | Unknown           |                  |                  |
| Moving-part safety                                                           | Unknown-->Pass    |                  |                  |
| Cost ≤ $300                                                                  | Unknown           |                  |                  |
| Lab usability ≤ 30 min                                                       | Unknown-->Pass    |                  |                  |

# Candidate Design 1

## Tabletop fit 500×250 mm
- **Discussion:** The spec requires a "turn centreline radius ≤ 800 mm." The physical path of a curve with an 800 mm radius alone requires a footprint much larger than 500×250 mm. Adding a ramp and straight sections makes it even larger.
## Turn Geometry
- **Discussion:** A physical curved road module (as sketched) perfectly satisfies this. When the vehicle travels through the curve, the physical track forces the outer wheels to travel a longer distance than the inner wheels, and the front axle to travel a different distance than the rear axle. This provides the most intuitive demonstration of differential kinematics.
## Full-time vs part-time 4WD in a turn
- **Discussion:** Because the vehicle is navigating a real physical curve, the demonstration will be highly visible. In part-time 4WD (locked center differential), the lack of speed difference between front and rear axles will cause drivetrain binding and visible tire scrub/slip. In full-time 4WD, the vehicle will turn smoothly.
## D3 locked axle in a turn
- **Discussion:** If the model includes a mechanism to lock the front or rear differential, driving it through the curved module will force the inner and outer wheels on that axle to rotate at the same speed. This will result in obvious tire scrub and increased turning resistance, perfectly demonstrating the D3 requirement.
## Input ≤ 2.5 N·m
- **Discussion:** The initial check correctly flags this. Driving on a flat surface requires very little torque. However, the ramp introduces a gravity component (climbing resistance). If the vehicle is too heavy, the incline is too steep, or the drivetrain friction is high, the manual hand crank (as sketched) might require more than 2.5 N·m of torque, making it too difficult for students to operate safely.
- **Action/Workaround:** Perform a torque calculation: `Required Torque = (Rolling Resistance + Climbing Resistance) × Wheel Radius / Total Gear Ratio`. If it exceeds 2.5 N·m, consider reducing the ramp angle, reducing vehicle weight, or using a geared DC motor instead of a hand crank to keep the input torque artificially low while maintaining the required speed.
## Moving-part safety
- **Discussion:** The sketch shows an adjustable slope and thin support rods (like a jack mechanism). Several safety hazards exist:
	- Are there pinch points in the ramp's lifting mechanism?
	- If the vehicle loses traction and slides down the ramp, is there a physical barrier?
	- Are the exposed gears and driveshafts properly guarded?
- **Action/Workaround:** During CAD development, enclose all gear meshes with clear acrylic guards. Ensure the ramp adjustment mechanism uses a safe lead screw or locking pins rather than exposed scissor mechanisms.
## Cost ≤ $300
- **Discussion:** CD1 has the highest potential cost among the candidates. Building multiple track modules (smooth, rough, curved), plus a ramp with an adjustable elevation mechanism, requires a lot of material (sheet metal, laser-cut wood, 3D printing, and hardware).
- **Action/Workaround:** Use standard aluminum extrusions and laser-cut acrylic/plywood to keep costs down. For the curved track, instead of a solid piece, just use a curved guardrail or slot to guide the wheels, saving material.
## Lab usability ≤ 30 min (Setup 15m + Test 15m)
- **Discussion:** The spec requires setup in 15 minutes. If students have to assemble the track using screws and bolts, this will consume the entire lab session.
- **Action/Workaround:** The track modules MUST use quick-release mechanisms (e.g., **magnets, dovetail joints, or snap-fit clips**). The transition between the flat track and the curved track needs to be seamless and tool-less.
# Candidate Design 2

# Candidate Design 3