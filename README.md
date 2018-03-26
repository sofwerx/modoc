# modoc
Mavros Object Designed Only for Communication

# dependencies

There are build dependencies on
* roscpp
* mavros

# running

`roslaunch modoc modoc-mavros.launch`

modoc's launch file modoc-mavros.launch will attempt immediately to connect to a px4 master running
at `fcu_url`.  That url can be a serial port or a tcp/ip port, as described at the mavros wiki page

http://wiki.ros.org/mavros#Connection_URL

A serial port can be specified by a path to a serial character device with baud rate parameter included 
as follows `fcu_url:=/dev/ttyACM0:57600`

A udp part can be specified as UDP: udp://[bind_host][:port]@[remote_host][:port][/?ids=sysid,compid]


