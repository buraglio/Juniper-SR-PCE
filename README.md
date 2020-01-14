# Juniper-SR-PCE
### Juniper JunOS PCE Segment Routing testing

Included here are the Test configurations for PCE testing with Juniper JunOS as well as the Topology and Eve-NG Lab XML File. This repo consists of a 6 Router Lab utilizing Juniper JunOS for testing of PCE and PCEP with external Segment routing controllers. This should provide enough configuration to test PCE and PCEP against the Juniper JunOS series vSIMs. Password Secret for the configurations is root / Juniper

### Files and such

1. vmx* Juniper vmx configuration files as stored in the flash. Also usable in the "startup configuration" section of Eve-NG
2. Nokia PCE Lab.unl - the Eve-NG XML file that is the lab


### Diagrams and physical layout

The Physical layout of this test environment is detailed in this diagram. There are two virtualization platforms - one a dedicated EVE-NG bare metal server with significant horsepower. The second is a VMWare cluster that runs the Nokia NFM-P, NRC-P, NRCP, NFMP, and NRC in a redundant manner, which are out of scope for this repo. VSR-NRC runs in a raw KVM environment inside of Eve-NG until the BOF interfaces can be worked out in Eve for that particular hardware model.

The physical topology inside of eve-ng that comprises the test network looks roughly like this.  
![Virtual Router Topology](https://github.com/buraglio/Nokia-SR-PCE/blob/master/PCE%20Eve-NG%20Test%20Topology.png?raw=true "Virtual Router Topology")
