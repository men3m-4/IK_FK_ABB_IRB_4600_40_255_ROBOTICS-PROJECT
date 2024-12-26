# IK_FK_ABB_IRB_4600_40_255_ROBOTICS-PROJECT
The robot was successfully programmed to trace a  trajectory in the shape of "201147"  The final drawing was achieved with high accuracy,  demonstrating the effectiveness of the FK and IK  algorithms and the interpolation method

ZeroMQ remote API

https://www.coppeliarobotics.com/helpFiles/en/zmqRemoteApiOverview.htm


The ZeroMQ remote API is one of several ways an application can connect with CoppeliaSim.



The ZeroMQ remote API allows to control a simulation (or the simulator itself) from an external application or a remote hardware (e.g. real robot, remote computer, etc.). It offers all API functions also available via a CoppeliaSim script: this includes all regular API functions (i.e. sim.* -type functions), but also all API functions provided by plugins (e.g. simOMPL.*, simUI.*, simIK.*, etc.), if enabled.



The ZeroMQ remote API functions are interacting with CoppeliaSim via ZeroMQ and its interface plugin to CoppeliaSim and the ZMQ remote API add-on. All this happens in a hidden fashion to the user. The remote API can let one or several external applications interact with CoppeliaSim in a stepping (i.e. synchronized with each simulation step) or non-stepping way (i.e. the normal operation mode), and even remote control of the simulator is supported (e.g. remotely loading a scene, starting, pausing or stopping a simulation for instance).



Install client package


$ python3 -m pip install coppeliasim-zmqremoteapi-client


the ZeroMQ and CBOR dependencies will be automatically installed with the above command
