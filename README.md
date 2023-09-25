# cisco-lab-4-traditional-topology
**Data Center:**
Server 1 and 2 belongs to Vlan 70 - 10.41.2.0/24 network
DNS Server belongs to Vlan 700 - 10.41.3.0/24 network
Gateway of Vlan 70 and 700 will be in Internet-Firewall (INT-FW)
Server-1 and Server-2 belongs to Vlan 333 and 444 accordingly - 10.31.2.0/24 and 10.31.3.0/24 networks
Gateway of Vlan 333 and 444 will be in Server Firm L3 Switch (Server-Firm-SW)
Transit network of Datacenter will be 10.41.1.0/24 and broadcast domain will contain /29 subnet mask
Datacenter will get internet (8.8.8.8) from ISP Internet Link-3 through Internet Router (INT-RTR)
Datacenter will get data connectivity from BTCL through Core Router (CORE-RTR)

**Head Quarter:**
HQ PC2 and PC4 belongs to Vlan 60 - 10.51.2.0/24 network
HQ PC1 and PC3 belongs to Vlan 61 - 10.51.3.0/24 network
Gateway of Vlan 60 and 61 will be in L3 Core Switch (CORE-SW)
Transit network of Head Quarter will be 10.51.1.0/24 and broadcast domain will contain /29 subnet mask
Head Quarter will get internet (8.8.8.8) from AMBER-IT Internet through Core-Router (CORE-RTR)
Head Quarter will get data connectivity from BTCL through Core-Router (CORE-RTR)

**CTG Branch:**
Hosts and transit network in CTG Branch will be in 10.71.1.0/24
CTG Branch will get internet (8.8.8.8) through Datacenter connected by a tunnel
CTG Branch will get data connectivity from BTCL through CTG Core Roueter

**KHL Branch:**
Hosts and transit network in KHL Branch will be in 10.71.2.0/24
KHL Branch cannot access internet
KHL Branch will get data connectivity from BTCL through KHL Core Router

There will be three tunnel from datacenter Core Router to Head Quarter, CTG Branch and KHL Branch

![Screenshot 2023-09-25 124807](https://github.com/smsufi/cisco-lab-4-traditional-topology/assets/39963872/f0672251-6d39-4188-9d34-85e9d76be46a)
