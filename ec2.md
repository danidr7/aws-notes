
# Elastic Compute Cloud

- Provides resizable compute capacity
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