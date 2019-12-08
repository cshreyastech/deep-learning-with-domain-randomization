# deep-learning-with-domain-randomization

Run validation:
cd /home/user/catkin\_ws
rm -rf build/ devel/
catkin\_make
source devel/setup.bash
rospack profile
roslaunch my\_dcnn\_training\_pkg start\_fetch\_randomenv\_ex4-3.launch
