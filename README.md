# rosserial-umd

## Setting up the communication protocol between Arduino and ROS:
### Prerequisites:
1. Download and install [Arduino IDE](http://arduino.cc/en/Main/Software). _Installing it in the `home` folder will be handy._
2. 


*Note: The `rosserial` ROS bindings are implemented as an Arduino Library. Like all other `Arduino Libraries`, `ros_lib` works by putting its library implementation into the `libraries' folder of your Arduino Sketchbook (Sketchbook location is a standard place to store Arduino programs, commonly known as sketeches).*




To install rosserial libraries in your own code/sketch, you must add the header file (Must be on the top!):
``
#include<ros.h>
`` 
before any other header file like `#include<std_msgs/String.h>`, else he Arduino IDE will not be able to locate them.



**

### Installing the `rosserial` libraries for arduino:

1. Using the `Advanced Packaging Tool`: (Highly recommended)
``sudo apt-get install ros-kinetic-rosserial-arduino``
``sudo apt-get install ros-kinetic-rosserial``

*If you are using `indigo`, modify accordingly!*.

2. Installing from Source onto the ROS workstation:
`git clone` the `rosserial` lib and build using `catkin_make`. Follow this [rosserial-git](http://wiki.ros.org/rosserial_arduino/Tutorials/Arduino%20IDE%20Setup/#Installing_from_Source_onto_the_ROS_workstation)


