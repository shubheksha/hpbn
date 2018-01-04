# [Primer on Latency and Bandwidth](https://hpbn.co/primer-on-latency-and-bandwidth/)

Speed depends on two critical components:

## Latency:

The time from the source sending a packet to the destination receiving it

## Bandwidth

Maximum throughput of a logical or physical communication path  
![](https://hpbn.co/assets/diagrams/3394fb4dab93efdd5e49475316c9496f.svg)

## Components of Latency

There are many components that play a part in delivering the message from the sender to the receiver. These components are as follows:

* **Propagation Delay**: the amount of time required for a message to travel from the sender to the receiver; it's the distance the message travel divided by the speed of the signal in the medium.

* ** Transmission delay**: the amount of time it takes for all the bits that make a packet on to the link; it's a function of the packet's length \(no. of bits?\) and the rate at which the link transfers data. It's independent of the distance b/w the sender and receiver.

* **Processing delay: the** amount of time it takes to process the header of the packet, check for bit-level errors and determine it's destination. The packet has fields which help with each of these things.

* **Queuing delay**: the amount of time the packet spends in the buffer of the router while waiting to be delivered or processed.

**Latency = Propagation delay + Transmission delay + Processing delay + Queuing delay**

> Note: Network data rates are typically measured in bits per second \(bps\), whereas data rates for non-network equipment are typically shown in bytes per second \(Bps\). This is a common source of confusion, pay close attention to the units.

## Last Mile Latency

The most significant delay is often introduced during the very last part of a packet's journey, not while crossing continents and oceans.

## Bandwidth in Core Networks

As per my understanding, "core networks" here imply where the packet spends most of its time travelling - the backbone of the internet that form the core data paths. These can be optic fibres or metal wires. However, optic fibres have a significant advantage over metal wires which can have a high maintenance cost,   higher loss and more interference. Moreover, optical fibres can carry many different wavelengths of light through multiplexing. Thus they've more bandwidth.

## Bandwidth at Network Edge

The bandwidth at the edge of the network infrastructure \(where the packet leaves the core data paths\) is significantly lesser. It depends on a number of factors and the technology used.

