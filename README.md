# deep-learning-with-domain-randomization

## Run validation:
```
cd /home/user/catkin_ws
rm -rf build/ devel/
catkin_make
source devel/setup.bash
rospack profile
roslaunch my_dcnn_training_pkg start_fetch_randomenv_ex4-3.launch
```
