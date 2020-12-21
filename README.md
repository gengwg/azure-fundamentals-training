# azure-fundamentals-training

## Day 1

* scalability vs elasticity
  * elasticity == *dynamically* scale up/down, out/in
* default  region is close to you.
* crosss region is on azure high speed private network.

* level of responsibility
  * iaas/paas/saas
  * shared responsiblity model
  * saas only care about data and access

* region == collection of data centers
  * avg region has about 16 data centers
  * each data center == separate facility
  * not all regions equal
  * choose region based on:
    * services you need available to that region?
    * cost: e.g. west2 is less expensive
    * closest region?
    * compliance: e.g. canadian region
    * latency
    * region pairs at the same geography
    * us gov and china regions

* availability zones and sets
  * no cost to user. design problem
  * availability zone must be in the same region
  * single vm 99.9%.
* fault domains:
  * geography > region > zones > data centers > racks

* resource group. bucket. metadata
  * need backup
* private preview -> public preview -> general availability (GA)

* resize causes down time ~ 10 sec
  * need spin up new hardware
* k8s means 'captain' in greek
* vnet peering
  * routing table only
  * no encryption such as vpn
  * within azure private network
* connectivity
  * point to point
    * e.g. laptop vpn client
    * 120 Mbps
    * public Internet
  * site to site VPN
    * 1 Gbps
    * public Internet
  * Express route private connectivity
    * high speed dedicated connecitvity to azure
    * 1 - 10 Gpbs
    * need privider for fiber
    * costs ~ 50k/mon
* storage account name must be globally unique within azure storage
* 3 copies of data. 
  * 2 copies for internal SLA purpose.
* GRS has 6 copies
  * 3 in current region; 3 in peering region.
  * note: egress charge for initial replication
  * storage cost + transaction cost
* ZRS: zone-redundant storage
* GRS: Geo-redundant storage
* ARM: azure resource manager
* a inch deep, a mile wide.

## Day 2

