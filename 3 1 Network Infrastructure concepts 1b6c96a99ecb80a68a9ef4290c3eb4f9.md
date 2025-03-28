# 3.1 Network Infrastructure concepts

Created time: 14 mars 2025 17:01
Last edited by: OLB_
Last edited time: 14 mars 2025 18:06

- Physical  isolation
    - different devices
    - different racks generally
    - can isolate customers and not mixing data between networks
    - could communicate but generally not
- Physical segmentation
    - differents switches. 1 per  customer
    - same rack
    - communication is controled
- Logical segmentation
    - VLANs in the same device / switch
    - 1 switch for 2 customers
- SDN (Software Defined Networking) - (model for building Software Network devices)
    - 3 layers: Data , control and management plane
    - Data plane : process the frames, encrypt, NAT
    - Control plane : control data plane actions, provide : routing tables, NAT tables, Dynamic Routing rules
    - Management Plane: configure the device, Web UI, SSH, SNMP