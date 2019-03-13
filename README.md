# crazyproto
Crazy ideas for electronics prototyping. Sometime we just have fun with it.

Projects:

**Hex-SOT23** Can we use hexagonal circuit traces to define a fixed layout to route a non-trivial circuit to a SOT23 footprint (e.g. NPN Bipolar transistor) such that the component placement alone defines the circuit?

![Node layout](https://github.com/sobuildit/crazyproto/blob/master/HEX-SOT23/hex_tile_node_assignment_50pc.png)

The concept is simple enough, the nodes (or wires/pads) in the centre {1,2,3} are the device pins, as identified on the PCB. The connection nodes are {A,B,C} and the 'power' nodes are {Vcc,Gnd} but those are just names, you can use them for anything.

The hex tiles with a single label present the same signal on both sides of the PCB.
The hex tiles with two labels present the top signal on the top surface and the bottom signal on the bottom. No surprises.

Finally, nodes of the form <letter><number> e.g. A2 are uncommitted nodes, that are useful for intermediate signals, and have no association with a connector pin or device pin.

The schematic is rough. Really rough (this is only a toy!) Also, the PCB design is also only a quick lashup and is drawn by hand, for fun. Gerbers are provided as-is, have not yet been manufactured, but I may do so in the future.

Do not use for RF! Parasitics will be off-the-chart bad!

![PCB Top 3D](https://github.com/sobuildit/crazyproto/blob/master/HEX-SOT23/Crazy-proto-SOT23-Top-3D.png)
Cost from allpcb, for quantity 10, HASL finish is estimated at about $24 USD before import duty, for the UK. Your country may differ. Have fun!
