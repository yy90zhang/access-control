# access-control
Source code for the paper "Smart contract-based access control for the IoT". 

Smart contracts:
ACC: Access Control Contract, one per subject-object pair
JC: Judge Contract, called by ACC(s) to judge the misbehavior of subjects and return the corresponding penalty.
RC: Register Contract, registering required information, such contract address and ABI for interacting with the ACCs and JC.

Javascripts:
registerACC: registering an ACC in the JC.
access_request: retriving the required information of an ACC and sending access reqeusts to this ACC for access control.
access_monitor: called by an object to watch the deployed ACC and retrive the access result when an access reqeust comes. 

