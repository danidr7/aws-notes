
# Elastic Block Store

- It's a virtual drive in the cloud.
- It provides persistent block storage volumes.
- Automatically replicated in the own AZ to protect against failure.
- Possibility of change an EBS volume on the fly.
- when attaching a volume to an instance, the volume must be in the same AZ as EC2.

### There are 5 flavors of EBS:
- General purpose SSD (gp2)
	- Good for most workloads
	- Balances price and performance
	- 16000 IOPS/volume
- Provisioned IOPS SSD (io1)
	- Good for databases.
	- The highest performance SSD volume
	- 64000 IOPS/volume
- Throughput Optimised Hard Disk Drive (st1)
	- Good for big data and data warehouses
	- Throughput optimized
	- 500 IOPS/volume
- Cold Hard Disk Drive (sc1)
	- Good for file servers
	- Designed for less frequently access workloads
	- 250 IOPS/volume
- Magnetic (Standard)
	- previous generation HDD
	- 40-200 IOPS/volume


## EBS vs Instance Store

- Instance Store Volumes are called Ephemeral Storage
- Instance Store cannot be stopper, if stopped all the data will be lost
- EBS backed instances can be stopped safely without lose data
- Both can be rebooted without lose the data
- By default both root volumes will be deleted on termination, but EBS allows to keep the root device.

## Snapshots

- Snapshots are a point in time copies of volumes
- They are incremental, only changed blocks since the last snapshot are moved to S3
- It's a good practice, before create a snapshot, stop the EBS that serve as root device

2 types of virtualization:
- HVM (Hardware Virtual Machine)
	- much more options of EC2 instances
- PV (Paravirtual)

Migrating a EBS to another AZ:
- Create a snapshot
- This snapshot will be available in AMI (Amazon Machine Image)
- Launch the snapshot in another AZ

It's possible to copy the AMI from a region to another