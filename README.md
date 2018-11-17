# Puppet

My goal is to bootstrap a whole openstack on cheap dedicated server from Hetzner & Online.net providers. As I have only a few dedicated servers and some instances from OVH Public Cloud, I need to make some adjustments to get everything working.

Of course I could use all the stuff on Puppet-Forge but my second goal is to train on puppet, so using something already existing is not in the scope.

My infra is for now composed of :
* 2 dedicated servers used for the control plane (all services needed to run an Openstack Cloud). Each OS component is runned inside a QEMU VM (KVM) managed directly by virsh.
* 3 dedicated servers used as compute hosts for openstack
* 2 OVH public cloud instances with RIPE IP block inside the vrack to give all the OS instance a public IP (flotting IP)
* 1 OVH public cloud instance to take care of puppet & ansible. it also works as a SSH gateway for all other servers

As I run everything on some cheap hardware I won't always fulfill all the OS requirement, in such case I will try some solution to go throught and get everything working.

Everything put on this repo is just the work of a beginner, so I won't recommand to use in any professional project.
