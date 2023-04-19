## Containers

To simplify the deployment of this, I'm building a series of container images to perform the functionality of the ocp-helper node.

- DNS
- DHCP
- Load Balancing
- HTTP Content for boot

In the original configuration, those services were provided by bind, dhcpd, haproxy and apache.  We will look to each of these and how we can collaboratively provide content for the controller and worker nodes in the OpenShift network.

TODO: define how many containers and the overhead required for each.
- Initial helper node has 6gb of ram, do we need all of that.
- Have the 