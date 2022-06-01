# Shared Planner

The SharedPlanner is a global planner plugin for the Nav2 Planner server. It implements the Navigation Function planner with either A\* or Dij. expansions. It is largely equivalent to its counterpart in ROS 1 Navigation. The Shared planner assumes a circular robot (or a robot that can be approximated as circular for the purposes of global path planning) and operates on a weighted costmap.

The `global_planner` package from ROS (1) is a refactor on Shared to make it more easily understandable, but it lacks in run-time performance and introduces suboptimal behaviors. As Shared has been extremely stable for about 10 years at the time of porting, the maintainers felt no compelling reason to port over another, largely equivalent (but poorer functioning) planner. 

See its [Configuration Guide Page](https://navigation.ros.org/configuration/packages/configuring-shared.html) for additional parameter descriptions.
