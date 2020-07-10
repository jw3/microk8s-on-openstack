microk8s on openstack
===

Microk8s cluster setup on OpenStack

### setup

Create an OpenStack network and subnet

- subnet address: `10.10.10.0/24`
- subnet nameservers:
```
8.8.8.8
8.8.4.4
```

Mandatory environment variables
  * `OS_*`: OpenStack environment, eg. `OS_AUTH_URL`, `OS_USERNAME`, ...
  * `KEY`: Name of OpenStack SSH keypair
  * `NETWORK_ID`: UUID of network
  * `ROUTER_ID`: UUID of router
  * `SUBNET_ID`: UUID of subnet

### reference

- OpenStack roles https://github.com/infraly/k8s-on-openstack
