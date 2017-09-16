.. _chapter_basicManeuvers:

Basic Maneuvers
===============

Are you ready to make the TurtleBot3 perform basic actions like moving forward, backward, turning right, left and stop?

It's quite simple in Blockly. You just need to select the appropriate block from the list of blocks available. Let's look at each of the basic actions and program the TurtleBot3 to move accordingly. 

Moving Forward
**************

.. image:: ystatic/mv_frwd.png


This block makes the TurtleBot3 move forward in three preset speed values - **SLOW**, **NORMAL** and **FAST**. Behind this block there is a short piece of code in `Python <https://www.python.org/>`_ that talks to the robot from the Blockly web interface and commands it to move forward with one of the preset values as programmed by the user. The figure below shows how the block is dragged into the workspace and the preset speed values are changed. 


.. image:: ystatic/fwd_mv.gif


The other basic maneuver blocks of the TurtleBot3 are shown in the following figures.

Moving Backward
***************

.. image:: ystatic/mv_bk.png


.. image:: ystatic/bk_mv.gif



Turning Right
*************

.. image:: ystatic/right.png


.. image:: ystatic/right_turn.gif


Turning Left
************

.. image:: ystatic/left.png


.. image:: ystatic/left_turn.gif


Turn Left/Right in degrees
**************************

All the above commands move the TurtleBot3 for a preset amount of time. To turn the TurtleBot3 a specific amount you can use the **Turn Left/Right __ degrees** command. Left turn is counter-clockwise and right turn is clockwise direction. This block uses the data from an Inertial Measurement Unit (IMU) sensor.

.. image:: ystatic/turn_lr_degrees.png


.. image:: ystatic/turn_lr_deg.gif



Stop
****

.. image:: ystatic/stop.png


.. image:: ystatic/stop_block.gif




