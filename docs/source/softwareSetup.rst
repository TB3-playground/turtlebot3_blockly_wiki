.. _chapter_softwareSetup:

Software Setup
==============

This section on software setup is intended for advanced users who would like to create custom blocks to either add new funtionalities or modify the existing ones.

The following steps were adapted from the instructions provided by `Erle Robotics <http://erlerobotics.com/blog/>`_.


Installation
************

Linux
~~~~~

Open terminal and enter the following instructions to install and develop blockly.
::

    $ mkdir -p ~/blockly_ws/src
    $ cd ~/blockly_ws/src
    $ git clone https://github.com/dabit-industries/turtlebot3_blockly
    $ cd turtlebot3_blockly/frontend/
    $ git submodule add https://github.com/dabit-industries/ace-builds.git ace-builds
    $ git submodule init
    $ git submodule update
    $ git submodule add https://github.com/dabit-industries/blockly.git blockly
    $ git submodule init
    $ git submodule update
    $ cd ~/blockly_ws/
    $ catkin_make_isolated -j2 --pkg turtlebot3_blockly --install

**or**
::

    $ mkdir -p ~/blockly_ws/src
    $ cd ~/blockly_ws/src
    $ git clone --recurse-submodules https://github.com/dabit-industries/turtlebot3_blockly
    $ cd ~/blockly_ws
    $ catkin_make_isolated -j2 --pkg turtlebot3_blockly --install

Launch
******
::

    $ source ~/blockly_ws/devel_isolated/setup.bash
    $ roslaunch turtlebot3_blockly turtlebot3_blockly.launch

.. NOTE::
  To launch the web interface of blockly, you don't necessarily have to start ``roscore`` but you should if you plan to connect TurtleBot3 and test it during development.
