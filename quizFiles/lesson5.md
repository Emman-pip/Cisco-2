# Lesson 5: STP
Q: a loop-prevention network protocol that allows for redundancy while creating a loop-free Layer 2 topology.
A: spanning tree protocol or STP

Q: STP is defined by IEEE 801.__
A: 1D

Q:  When multiple paths exist between two devices on an Ethernet network, and there is no spanning tree implementation on the switches, a ______ occurs
A: layer 2 loop

Q: (t/f) A Layer 2 loop can result in MAC address table instability, link saturation, and high CPU utilization on switches and end-devices, resulting in the network becoming unusable.
A: t

Q: is an abnormally high number of broadcasts overwhelming the network during a specific amount of time.
A: broadcast storm

Q: who wrote the paper "An Algorithm for Distributed Computation of a Spanning Tree in an Extended LAN"
A: Radia Perlman

Q: STP is based on ___
A: spannning algorithm or STA

Q: switches use _____ to share information about themselves and their conenctions
A: bridge protocol data units or BPDU

# BPDUs contain a BID

Q: components of bridge ID
A: bridge priority, extended system ID, MAC address

Q: default priority for all cisco switches
A: 32768

Q: range of bridge priority
A: 0 to 61440

Q: bridge priority is incremented by ____
A: 4096

Q: (t/f) A bridge priority of 0 does not take over all other bridge priorities
A: f

Q: is a decimal value added to the bridge priority value in the BID to identify the VLAN for this BPDU.
A: extended system ID

Q: allows later implementations of STP to have different root bridges for different sets of VLANs.
A: extended system ID

Q: When two switches are configured with the same priority and have the same extended system ID, the switch having the ________ with the lowest value, expressed in hexadecimal, will have the lower BID.
A: MAC address

Q: After a switch boots, it begins to send out BPDU frames every ___ seconds
A: 2

Q: The _______ are defined by the speed at which the port operates
A: default port costs

Q: The path information, known as the ____________, is determined by the sum of all the individual port costs along the path from the switch to the root bridge.
A: internal root path cost

Q: The _____ is the port closest to the root bridge in terms of overall cost (best path) to the root bridge. This overall cost is known as the internal root path cost.
A: root port

Q: is equal to the sum of all the port costs along the path to the root bridge
A: internal root path cost

Q: (t/f) Every segment between two switches will have one designated port.
A: t

Q: f a port is not a root port or a designated port, then it becomes an _____ port
A: alternate or backup

Q: is the interval between BPDUs. The default is 2 seconds but can be modified to between 1 and 10 seconds.
A: hello timer

Q: is the time that is spent in the listening and learning state. The default is 15 seconds but can be modified to between 4 and 30 seconds.
A: forward delay timer

Q: is the maximum length of time that a switch waits before attempting to change the STP topology. The default is 20 seconds but be modified to between 6 and 40 seconds.
A: max age timer

Q: default max age timer
A: 20

Q: STP states
A: disabled, blocking, listening, learning, forwarding

Q: (STP port state) only receives BPDU
A: blocking

Q: (STP port state) receive and send BPSU no updates in MAC address and no fowarding
A: listening

Q: (STP port state) receive and send BPSU updates in MAC address and no fowarding
A: learning

Q: (STP port state) receive and send BPSU updates in MAC address and fowarding
A: forwarding

Q: (STP port state) no activity at all
A: disabled

Q: In ______ versions of STP, there is a root bridge elected for each spanning tree instance.
A: per-vlan spanning tree or PVST

Q: without any configurations on a switch, what will be the basis for electing the root bridhe
A: MAC address

Q: The root bridge will be the switch with the:
A: lowest bridge ID

Q: the original IEEE 802.1D standard
A: STP

Q: STP is also called ____
A: common spanning tree or CST

Q: it assumes one spanning tree instance for the entire bridged network, regardless of the number of VLANs
A: STP OR CST

Q: is a Cisco enhancement of STP that provides 802.1D spanning tree instance for each VLAN configured in the network
A: per-VLAN spanning tree or PVST+

Q: evolution STP that provides faster convergence than STP
A: RSTP

Q: RSTP is known by the standard IEEE 801.__
A: 1w

Q: an updated version of the STP standard, incorporating IEEE 802.1w
A: 801.1D-2004

Q: cisco enhancement of RSTP that uses 802.1w per VLAN
A: Rapid PVST+

Q: is an IEEE standard inspired by the earlier Cisco proprietary Multiple Instance STP (MISTP)
A: multiple spanning tree protocol or MSTP

Q: is the cisco implementation of MSTP, which provides up to 16 instances of RSTP and combines many VLANs with the same physical and logical topology into a common RSTP instance
A: multiple spanning tree or MST

Q: RSTP port states
A: Discarding, learning, forwarding

Q: equivalent of discarding port in STP
A: disabled, blocking, listening

Q: equivalent of blocked port in RSTP
A: backup and alternate port

Q: When a switch port is configured with _____, that port transitions from blocking to forwarding state immediately, bypassing the usual 802.1D STP transition states (the listening and learning states) and avoiding a 30 second delay.
A: PortFast

Q: (t/f) PortFase can be used to a port connecting to another switch
A: f

Q: _____ immediately puts the switch port in an errdisabled (error-disabled) state on receipt of any BPDU
A: BPDU Guard




