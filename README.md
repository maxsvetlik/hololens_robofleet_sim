# hololens_robofleet_sim

A hopfully simplified simulation experience for running the robofleet pipeline offline.

## Installation

$ git clone https://github.com/maxsvetlik/hololens_robofleet_sim.git --recursive

Each component should be run, build according to their own READMEs...

$ cd hololens_robofleet_sim/robofleet_server && yarn install && yarn build

$ cd ../robofleet_client && make

$ cd ../cpp_client/robofleet_client && make 

# Running

For now, need to run each component in its own terminal. If in the root of this repo
the following commands will bring everything up:

1. $ roscore
1. $ cd robofleet_server && yarn start 
1. $ ./robofleet_client/scripts/basic_status.py 
1. $ cd robofleet_client/ && ROS_NAMESPACE="maxbot1" make run 
1. $ cd cpp_client/robofleet_client/ && make run 
