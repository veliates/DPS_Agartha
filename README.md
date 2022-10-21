# DPS_Agartha

## Team Members
- *Tural Hasanov*
- *Veli Ates*
- *Rahim Hashimov*
- *Sadiya Yesmin*
- *Seda Sensoy*

### Protocol
> Protcol information

### Data/signal/events are required for the interaction / communication between the trucks
#### Signals:
- __Break__: 
- __Decelerate__: Decrease speed of all trucks at the same rate 
- __Accelerate__: Increase speed of all trucks at the same rate 
- __Break Acknowledge__: The braking vehicle then sends out ACK (Acknowledge). Preceding vehicles can thus start to brake when the ACK from succeeding cliques arrives. Front vehicle cannot brake until ACK is received from rear that it has started to brake.

#### Data:
- __Speed__
- __Gap Distance__
- __Acceleration__
- __GPS Coordinates__
