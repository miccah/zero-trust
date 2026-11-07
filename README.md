# Zero Trust Networks

Notes for *[Zero Trust Networks](https://www.oreilly.com/library/view/zero-trust-networks/9781492096580/)*
by Razi Rais, Christina Morillo, Evan Gilman, and Doug Barth.


## Table of Contents

* [Fundamentals](#fundamentals)


## Fundamentals

There are 5 fundamentals that zero trust networks are built on:

* The network is always hostile
* There are always external and internal threats on the network
* Network locality alone is not sufficient for trusting a network
* Every device, user, and network flow is authenticated and authorized
* Policies should be dynamic and calculated from as much information as possible

A traditional network often uses zones with firewalls in between, but with
zero trust, network location does not matter. This means a VPN is not
necessary, and all servers can exist on the open internet. All that is required
is a control plane.


### Control plane

The control plane in a zero trust network coordinates and controls the data
plane, which are servers and other resources. Requests for access to protected
resources are first made through the control plane. Once approved, the control
plane dynamically configures the data plane to accept traffic from the approved
client. This decision is time-bound, so the control plane may revoke access.

The basic idea of a control plane is that an authoritative source has the
ability to authenticate, authorize, and coordinate access in real time, based
on a variety of inputs.
