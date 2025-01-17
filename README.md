# Quatt-CiC-hack
This is a collection of Home Assistant automations that will allow more control over your Quatt.io heat pump than with the Quatt CiC App

The idea was taken from collected knowledge on the Tweakers forum for Quatt users. See also: https://gathering.tweakers.net/forum/view_message/81286482

The Quatt CiC control algorithm is known to use the difference in temperature between the actual room temperature (as seen by your thermostat) and the room setpoint as the main driver and the outside temperature and possibly other parameters as minor drivers.
The Quat CiC is only controlling the compressor level (levels 0-10) and the water pump speed. Other actions the Quatt heat pump will perform such as defrosts, bottom plate heater, crank case heater, e.a. are not controlled by the CiC but by the controller board inside the Quatt monobloc outside unit (see www.quatt.io)
See also: https://gathering.tweakers.net/forum/view_message/81285528

The HA automations are:
[1] When thermostat heating is ON then thermostat-room-setpoint follow thermostat-room-temperature plus offset
[2] Change Offset on change in ComprLevel or ComprLevelDemand until ComprLevel equal ComprLevelDemand





