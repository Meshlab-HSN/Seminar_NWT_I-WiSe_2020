Tasks for each team to be performed.
Uploading data is done by opening a new pull request.

- [x] Upload your presentation (to your team folder)
- [x] Generate one ssh key pair (public & private key) for your team
- [x] Upload your public ssh key (to your team folder)
- [x] Check ssh connectivity to your VM
- [x] Prepare your demo

First goals: 
Get 2 virtual OpenWRTs and one QEMU bridge running via QEMU. (done)
Configure virtual network (done)

Demo explanation:
On the host virtual machine, qemu is used to virtualize one OpenWrt-based server node and three OpenWrt-based client nodes. Those are connected to a qemu-managed bridge on the host and establish a virtual isolated network. The qemu bridge is based on a bridge interface on the host. If everything is configured, these nodes need to be configured one-by-one, one acting as a DHCP server and the other ones acting as clients.
Afterwards, these nodes need to be started manually one-by-one and will then form a virtual network where the clients receive IP addresses from the server.
