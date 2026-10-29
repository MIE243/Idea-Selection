# Initial Check

| Categories                                                                   | CD1 (ramp/course) | CD2 (belt bench) | CD3 (hand crank) |
| ---------------------------------------------------------------------------- | ----------------- | ---------------- | ---------------- |
| Tabletop fit 500×250 mm                                                      |                   | Likely fail |                  |
| Turn geometry: (i) left/right and (ii) front/rear travel different distances |                   | (i) Left/right — Pass in simulation; (ii) Front/rear — Fail |                  |
| Full-time vs part-time 4WD in a turn                                         |                   | Fail |                  |
| D3 locked axle in a turn                                                     |                   | Without an axle lock — Fail; with an axle lock — Possible simulation |                  |
| Input ≤ 2.5 N·m                                                              |                   | Unknown |                  |
| Moving-part safety                                                           |                   | Fail |                  |
| Cost ≤ $300                                                                  |                   | May fail |                  |
| Lab usability ≤ 30 min                                                       |                   | Potentially pass |                  |

# Candidate Design 1

# Candidate Design 2

## 1. Tabletop fit 500 × 250 mm

**Likely fail as designed:** The vehicle and belt bench must share the 500 × 250 mm footprint. Belts, rollers, the frame and guards reduce the space available for the vehicle. If the vehicle is large enough for its drivetrain components to be clearly observed and handled, the complete bench may exceed the size limit. Reducing the vehicle size to make it fit may make drivetrain motion harder to observe and components harder to handle and replace. A dimensioned layout is needed to confirm the fit.

## 2. Turn geometry: (i) left/right and (ii) front/rear travel different distances

**(i) Left/right — Pass in simulation:** The two independently controlled belts can create different left and right wheel speeds, simulating the different distances travelled by the wheels on the same axle during a turn.

**(ii) Front/rear — Fail:** Each belt contacts both the front and rear wheels on the same side. Assuming equal wheel sizes and no significant slip, the bench cannot independently create the front/rear axle-speed difference required for a turn.

**Curved path — Fail:** The vehicle is held stationary and does not travel along a curved path, so the specified turn with a centreline radius of ≤ 800 mm is not demonstrated.

## 3. Full-time vs part-time 4WD in a turn

**Fail:** In the comparison specified here, full-time 4WD uses a centre differential that allows the front and rear axles to rotate at different speeds, while part-time 4WD in 4WD mode connects the front and rear outputs together and prevents that speed difference. The current two-belt bench cannot independently create the front/rear axle-speed difference needed to demonstrate the contrast: each belt contacts both the front and rear wheels on the same side. As a result, the bench cannot clearly show the centre differential accommodating different axle speeds or demonstrate the expected slip in part-time 4WD during a turn. The vehicle also remains stationary rather than travelling along the specified curved path.

## 4. D3 locked axle in a turn

**Without an axle lock — Fail:** The left and right wheels on the same axle cannot be deliberately locked to rotate at the same speed, so the bench cannot demonstrate the locked-axle condition required by D3.

**With an axle lock — Possible simulation:** The left and right belts can run at different speeds while the wheels are locked together. This may cause wheel-to-belt slip or increased resistance, but the effect must be verified. The vehicle remains stationary, so it does not follow the curved path specified in D3.

## 5. Input ≤ 2.5 N·m

**Not yet demonstrated:** CD2 uses two independently controlled electric motors to drive the left and right belts. The belts then rotate the vehicle's wheels through contact, transferring forces into the drivetrain. The torque required from each motor will depend on the belt and roller resistance, wheel-to-belt contact, drivetrain friction, and the selected operating condition. For example, a locked axle or unequal belt speeds may increase resistance or cause slip.

Because the system has two separate motor inputs, the team must clarify where and how the 2.5 N·m input-torque limit applies before deciding whether the design meets it. The required torque and speed should then be estimated for both motors and compared with their capabilities under the intended load. The selected motors' rated torques alone are not enough to demonstrate compliance, because operating torque can vary with load. A suitable calculation or test is needed to confirm the result.

## 6. Moving-part safety

**Fail:** The CD2 concept includes moving belts, support rollers, wheels, gears and shafts. The points where the belts enter the rollers are potential pinch points: a finger or clothing placed near the contact area could be drawn between the moving belt and roller. The wheel–belt contact areas and gaps between moving parts and the frame also need to be assessed. Although a transparent cover is shown around part of the drivetrain, the illustration does not show complete guarding around the belts, wheels and roller contact points. The run/stop controls do not prevent direct access to these hazards. Transparent guards or other barriers are needed to prevent finger access while keeping the drivetrain visible. The completed design must be checked for accessible openings and clearances before it can be considered safe.

## 7. Cost ≤ $300

**May fail — at risk of exceeding CAD $300:** CD2 requires both the vehicle drivetrain and a two-belt demonstration bench. The bench adds costs for motors, motor controllers, a power supply, belts, rollers, a frame and safety guards.

As an initial price reference, two geared motors would cost approximately CAD $56.70 ([CAD $28.35 each](https://ca.robotshop.com/products/e-s-motor-dc-flat-spur-gear-motor-parallel-shaft-gear-motor-12v-64rpm)), two motor controllers approximately CAD $36.70 ([CAD $18.35 each](https://ca.robotshop.com/products/cytron-13a-5-30v-single-dc-motor-controller)), and one 1 kg spool of PLA approximately [CAD $15.49](https://ca.robotshop.com/products/3d-printing-canada-usa-black-budget-pla-filament-175mm-1kg). These items total approximately CAD $108.89, leaving CAD $191.11 for the remaining components before shipping and taxes.

These prices are examples for comparison; cheaper suitable alternatives may be available. However, the belts, power supply, drivetrain hardware, guards and any axle-lock mechanism still need to be priced, and the suitability of the example components must be checked. Therefore, the complete design cannot yet be confirmed to meet the CAD $300 limit.

## 8. Lab usability ≤ 30 min

**Potentially passes:** CD2 keeps the vehicle stationary on a bench, and students can use the belt-speed controls and selector lever to change operating conditions and compare drivetrain motion. This could allow four students to complete the setup and demonstration within the target of 30 minutes: approximately 15 minutes for setup and 15 minutes for testing. However, the required demonstration functions are not yet fully established. Any additional axle lock, drivetrain input or safety guards may affect setup and switching time. A timed four-student trial is needed to confirm whether the complete procedure meets the target.

# Candidate Design 3
