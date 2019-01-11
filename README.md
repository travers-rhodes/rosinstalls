# rosinstalls
Rosinstall files. This repo is public so that initializing new workspaces is a one-liner.

'''
cd ~
mkdir my_catkin_ws
cd my_catkin_ws
wstool init src https://raw.githubusercontent.com/travers-rhodes/rosinstalls/master/ur5.rosinstall
wstool update
rosdep update
rosdep install --from-paths src --ignore-src -r -y
catkin_make
source devel/setup.bash
'''

See https://github.com/personalrobotics/pr-rosinstalls for excellent further instructions.
