# ansible-workshop
Red Hat Public Sector's Ansible workshop using AWS

## Slide deck
You can read the slide deck [here](https://docs.google.com/presentation/d/1t9ItFtOOufZ7UyMuAJC2GVk0JfU-u1nX698Skn00CA8/edit?usp=sharing).

## Requirements
This requires Ansible 2.1, which is included in the workshop AMI. We also use the ec2_vpc_peer module, which is in this repo at [library/ec2_vpc_peer.py](https://github.com/jason-callaway/ansible-workshop/blob/master/library/ec2_vpc_peer.py).

## Known issues
There appears to be a race condition with the creation of a VPC and the modification of its Route Tables. If your playbook run fails aound this point, just re-run until it completes. I believe this to be a bug with the EC2 API, and not something that can be fixed except with pauses.

## Contact
If you'd like to attend this workshop, contact [Jason Callaway](mailto:jcallawa@redhat.com).
