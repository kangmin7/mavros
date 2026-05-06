# MAVROS for m-explore-ros2

Custom [MAVROS](https://github.com/mavlink/mavros) for integration with [m-explore-ros2](https://github.com/robo-friends/m-explore-ros2), targeting ROS 2 Humble

---

## Changes

- added `use_sim_time` parameter to `node.launch` and `px4.launch` (default: `false`)
- Local position frame changed from `map` to `odom`, with TF publishing enabled (`map → odom → base_link`)

---

## Running

```bash
ros2 launch mavros px4.launch fcu_url:=udp://:14540@127.0.0.1:14557 use_sim_time:=true
```
