# WIP (Do not use)

# growing-framework
ESP-IDF based framework for full growing cycle automation

General idea is to build fully automated and horyzontaly clustered aqua/hydro/fog/aero-ponics which can work with cheap hardware.

### Node
Separate growing instance of any size, that can make decidions, based on internal metrics and configuration.
Is self-sustained, and can be fully functional without external control.
Can be separate pot, growbox, room, etc.

### Cluster
Nodes can be connected to clusters in a Master-Master or Master-Slave mode.
Cluster behaves like a single node.
General purpose of cluster is to make centralized heating/lightning system and make decidions based on aggregated data, which is not accesible to a single node. (Like CO2 concentration or EC/PH level).


### IoT backend
Master Nodes are connected to IoT backend for a few reasons:
* remote control _(declarative way)_
* access external data, like weather forecast
* send metrics and logs _(like: 11:19AM injected 10ml of `N` nutrient)_

Growing stages are controlled by backend using the remote control functionality
