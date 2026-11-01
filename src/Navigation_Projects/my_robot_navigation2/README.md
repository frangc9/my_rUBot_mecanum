# AUTONOMOUS NAVIGATION EVALUATION 
## Mecanum Project - Activity 5, Part 3

Autonomous navigation with Nav2 has been validated in the simulated environment `group4_custom.world` using the generated map `group4_map` and the parameter file `rubot_sw_ign.yaml`.
The evaluation was carried out across multiple trials, testing distinct routes toward each of the designated reachable areas of the map.


### Verifications Performed:
1. **Global Path:** The planned trajectory remains entirely within the mapped free space without traversing obstacles.
2. **Local Controller:** The robot tracks the path smoothly without sustained oscillations.
3. **Obstacle Avoidance:** Verified that the robot dynamically recalculates and avoids unforeseen obstacles along the route.
4. **Goal Reached:** The rUBot successfully reaches target poses set via `Nav2 Goal` while preserving safety margins from walls.
5. **AMCL Localization:** Pose estimation remains accurate and consistent with the simulated pose in Gazebo.

Thus, **modifying default parameters in** `rubot_sw_ign.yaml` **was unnecessary**, as inflation layers, robot footprint, and tolerances adequately meet safety and performance criteria.
