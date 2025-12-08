# MORAI Example ROS2

Check that your MORAI SIM is configured correctly for communicating over ROS2 with this open-source example project

## File structure
```
./
├── src          
│    ├── morai_ros2_connector     # script for MORAI Simulator to open ROS2 service
│    ├── morai_ros2_msgs          # MORAI Simulator ROS2 message set (submodule)
│    └── morai_sim_examples       # example ros2 nodes and unit testing code
└── morai_ros2_bridge_[version]   # bridge script to connect MORAI SIM with ROS2
```

## Requirements


| ROS 2 Version | Support |
|---|---|
| Eloquent | 🟢 |
| Foxy | 🟢 |
| Galactic | 🟢 |
| Humble | 🟢 (Updated 2025) |
| Jazzy | Working on it! |
| Kilted | Not planned |

- Ubuntu version should match the ROS 2 distro (e.g. Humble --> Ubuntu 22.04)
- Python version should also match the ROS 2 distro (e.g. Humble would by default match with Python 3.10)

## Setup

```
$ mkdir ~/ws_morai_sim_example
$ cd ~/ws_morai_sim_example
$ git clone https://github.com/MORAI-Autonomous/MORAI-Example-ROS2.git
$ source /opt/ros/<your ROS2 version>/setup.bash
$ colcon build
$ source ./install/setup.bash
```

## Use

```
$ source ./install/setup.bash
$ ./gRPC_ROS2_Bridge
```

## Resources

- [Website](https://www.morai.ai/)
- **Documentation**:
  - [MORAI SIM Manual (English)](https://morai-sim-drive-user-manual-en-24-r2.scrollhelp.site/morai-sim-drive-user-manual-en-24.r2/Working-version/?l=en)
  - [MORAI SIM Manual (Korean)](https://help-morai-sim.scrollhelp.site/)

## License and acknowledgements

This project is licensed under the [MIT License](LICENSE).
