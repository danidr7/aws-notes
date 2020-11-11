
# Identify and Access Management

 IAM allows to manage users and their accesses to AWS console.

- Control of AWS account
- Share account access
- Granular user permission
- Multi-factor Auth (very recommended for root user)
- temporary access for users/devices/services
- setup password rotation policy
- supports PCI DSS framework

- IAM doesn't have a region (it's universal)
- Root account is who created the account
- New users have no permissions
- New users are assigned for an access key and a secret access key when first created
	- these credentials can be view only once
 

## Terminology

Users: end user of the platform
Groups: a collection of users where share permissions
Policies: permissions for control what an user/group/role can do
Role: permissions for control what a resource can do