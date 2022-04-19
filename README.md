# system-temperature-control-protoimpl
A prototype that implements an open source speficiation for integrating a system temperature control module. Wow that's a lot of jargon.

Basically, theres a motherboard, with temperature sensors, fan IO, and power saving ~~bloatware~~ firmware, that basically just operates at some frequency of querying "if the equation (inputs: all temp sensors) outputs a temperature over some threashold, turn on these fans". But most devices exist not in some arbitrary cold environment, but usually share an environement with other devices. If feed back loops are possible, an external system should be granted the power of managing the network.

The specification would basically be a protocol for the motherboard to communicate with a network of other devices that interact with the local environment, and communicate. The environment is low on power? is the computer allowed to sleep now? what about the monitors? etc. basically a protocol to allow for those types of queries to and from devices based on network policies.
