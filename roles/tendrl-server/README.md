Tendrl Server
=============

This role automates installation of *Tendrl Server*, as described in *Server
Installation* section of [Tendrl Package Installation
Reference](https://github.com/Tendrl/documentation/wiki/Tendrl-Package-Installation-Reference)

Requirements
------------

This role expects that the repositories with Tendrl packages (and it's
dependencies) is already available on the machine.

Role Variables
--------------

* When `etcd_ip_address` variable is undefined (which is the default state),
  this role will use ip address of default ipv4 network interface to configure
  etcd, otherwise a value of this variable will be used.

* When `tendrl_ceph_provisioning_support` variable is True (default is False),
  Tendrl will be able to provision Ceph clusters via ceph-installer installed
  on Tendrl Server machine. When you enable this, make sure that repository
  with ceph-installer is available on this machine.

License
-------

Apache 2.0