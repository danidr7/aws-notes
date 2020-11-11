
# Elastic Compute Cloud

- Virtual machines in the cloud
- Provides resizable compute capacity
- reduce the time for obtain and boot a new instance
- Allows to quickly scale capacity

## Pricing Models

- **On Demand**
	- fixed rate by hour/second
	- no commitment
	- useful for:
		- low cost and flexible capacity
		- applications that cannot be stopped with unpredictable workloads
		- applications in development stage
- **Reserved**
	- capacity reservation
	- significant discount
	- contract terms 1 or 3 years
	- useful for:
		- predictable usage
		- applications that need reserved capacity
		- reduce costs with upfront payments
	- reserved pricing types:
		- **Standard**
			- 75% on demand instances
			- more discount with the more upfront is the payment
			- cannot change the instance type
		- **Convertible**
			- 54% on demand instances
			- capability to change the instance type
		- **Scheduled**
			- allows to scale within the time windows you reserve
- **Spot**
	- bid a price for an instance
	- the price is variable (like the stock market)
	- if the bid isn't above that price, then the instance is lost
	- even greater savings
	- partial hour of usage won't be charged when terminated by EC2
	- partial hour of usage will be charged when terminated by user
	- useful for:
		- applications with flexible start/end time
		- very low compute prices
		- for large amounts of additional capacity
- **Dedicated Hosts**
	- Physical dedicated EC2 server
	- help to reduce costs allowing to use server bound licenses
	- useful for:
		- regulatory requirements that may not support multi-tenant virtualization
		- take advantage of licensing
		- can be purchased on-demand (hourly) or as a reservation (70% off)

## Instances types

- Families: F1, I3, G3, H1, T3, D3, R5, M5, C5, P3, X1, Z1D, A1, U-6tb1
- Mnemonic:
	- **F**: for FPGA (Field Programmable Gate Array)
	- **I**: for IOPS
	- **G**: for Graphics intensive (video enconding)
	- **H**: for High Disk Throughput
	- **T**: for cheack general purpose 
	- **D**: for Density
	- **R**: for RAM
	- **M**: for main choice for general purpose
	- **C**: for Compute
	- **P**: for Graphics (machine learning)
	- **X**: for extreme memory
	- **Z**: for extreme memory and CPU
	- **A**: for arm-based workloads
	- **U**: for bare metal
- The number in the family is the generation of the instance