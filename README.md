# DPS Agartha

## Team Members
- *Tural Hasanov*
- *Veli Ates*
- *Rahim Hashimov*
- *Sadiya Yesmin*
- *Seda Sensoy*

### Protocol
> Vehicle-to-Vehicle (V2V) Communications is used for platooning. V2V augments other on-board sensors like radar and cameras by delivering instantaneous status updates
of vehicles outside line-of-sight. When compared to traditional adaptive cruise control (ACC) solutions exclusively based on radar, this increases the string stability
of the system of vehicles traveling together.

### Data/signal/events are required for the interaction / communication between the trucks
#### Signals:
- > __Break__: Decrease speed of all trucks at the same rate
- > __Accelerate__: Increase speed of all trucks at the same rate 
- > __Break Acknowledge__: The braking vehicle then sends out ACK (Acknowledge). Preceding vehicles can thus start to brake when the ACK from succeeding cliques arrives. Front vehicle cannot brake until ACK is received from rear that it has started to brake.

#### Data:
- __Speed__
- __Gap Distance__
- __Acceleration__
- __GPS Coordinates__
- __Blind Spot Monitoring__

#### Events
- > __Normal breaking__: This is a common occurrence in thick traffic while approaching a traffic congestion. Because of the traffic jam, the car in front of the platoon gradually slows down.
- > __Emergency breaking__: The driver may cause full braking (maximum braking) which is an event that shall be handled in the platoon.
- > __Cut-in__: The cut-in item (vehicle, motorbike, or truck) can appear anywhere in the platoon and for any length of time. A cut-out action occurs when the cut-in vehicle exits the platoon. The system's reaction may differ depending on the duration of the cut-in.
- > __Failure of the system__: Communication Loss.


### Communication Failure:
> Each vehicle decreases the value of speed separately when a communication loss is detected. To maintain stability the decrease rate must be the same for all
> vehicles. The rate is imposed by safety requirements in the worst communication loss scenario. All vehicles automatically switch to autonomous mode. Each vehicle
> begins decreasing the value of their speed with the maximum deceleration rate. So the vehicles behind the decelerating vehicle react exactly as if there were a
> communication even without knowing about the hard braking


### How can the distance to the precedence truck be guaranteed
> Adaptive cruise control is an available cruise control advanced driver-assistance system for road vehicles that automatically adjusts the vehicle speed to maintain a safe distance from vehicles ahead
>

