# nloptcontrol_planner

A stand-alone demo to show that the `NLOptControl.jl` is solving the OCP and connected to `ROS`.

## status = working

## To Run
```
roslaunch nloptcontrol_planner demo.launch
```

## Expected Output
After a few minutes the terminal should display:
```
******************************************************************************
This program contains Ipopt, a library for large-scale nonlinear optimization.
 Ipopt is released as open source code under the Eclipse Public License (EPL).
         For more information visit http://projects.coin-or.org/Ipopt
******************************************************************************

Running model for the: 0 time
[199.831, 8.44829, -0.304456, 0.225719, 1.62274, 0.0524729, 16.7114, -1.11083]
nloptcontrol_planner has been initialized.
Running model for the: 1 time
[198.976, 16.6123, -0.820356, 0.246638, 1.75329, 0.0330637, 16.1247, -1.22459]
Running model for the: 2 time
[197.441, 24.3947, -0.579523, 0.0349721, 1.8273, -0.00889783, 15.6299, -0.77718]
Running model for the: 3 time
[195.715, 31.9384, -0.0419052, -0.121407, 1.80044, -0.0317296, 15.3501, -0.361812]
Running model for the: 4 time
[194.294, 39.4512, 0.237982, -0.16141, 1.72634, -0.0360165, 15.2689, 0.0185792]
Running model for the: 5 time
[193.395, 47.0487, 0.302376, -0.149562, 1.64747, -0.0328082, 15.3683, 0.361693]
Running model for the: 6 time
[193.034, 54.7811, 0.269118, -0.117383, 1.58031, -0.0253441, 15.6244, 0.646153]
Running model for the: 7 time
[193.132, 62.6823, 0.204767, -0.0873723, 1.52942, -0.0189879, 16.0035, 0.854896]
Running model for the: 8 time
[193.601, 70.7833, 0.149901, -0.0649146, 1.49162, -0.0140566, 16.4672, 0.985584]
Running model for the: 9 time
[194.365, 79.1078, 0.10819, -0.0480866, 1.46356, -0.0102397, 16.9765, 1.03786]
Running model for the: 10 time
goal is in range
[195.357, 87.6683, 0.0590599, -0.020078, 1.44614, -0.00305557, 17.4935, 1.02433]
Running model for the: 11 time
goal is in range
[196.478, 96.4715, -0.0230271, 0.00710531, 1.44323, 0.00253812, 18.002, 1.00652]
Running model for the: 12 time
goal is in range
[197.629, 105.525, -0.100926, 0.0220395, 1.45104, 0.00503927, 18.5022, 0.990981]
Running model for the: 13 time
goal is in range
[198.736, 114.834, -0.150177, 0.027248, 1.46365, 0.00574419, 18.9955, 0.978923]
Running model for the: 14 time
goal is in range
[199.758, 124.4, -0.175388, 0.0281426, 1.47758, 0.00578579, 19.4841, 0.974316]
Goal Attained!

[obstacle_avoidance-2] process has finished cleanly
log file: /home/febbo/.ros/log/f7108cac-2de8-11e8-8052-104a7d04da99/obstacle_avoidance-2*.log
```

This indicates a successful test.

## Notes

  * A large optimization problem needs to be initialized
  * caching the functions upon start-up takes a few minutes
