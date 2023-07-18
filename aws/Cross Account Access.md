
Accessing services accross AWS accounts by using roles. 

1. Create a role in the target account (e.g hosting the resource(s) trying to be accessed) should mark the origin account (e.g. the account making the request) as a trusted account.
2. Create a role in the origin account and add the permission to assume role in target account
3. Attach the origin account role to the service (e.g EC2) to allow it access the resource in target account

Releates to: [[Role]]

 