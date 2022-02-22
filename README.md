# ansible-role-gvisor

Ansible role to install and configure gVisor Container runtime:
gVisor is an application kernel, written in Go, that implements a substantial
portion of the Linux system surface. It includes an Open Container Initiative
(OCI) runtime called runsc that provides an isolation boundary between the
application and the host kernel. The runsc runtime integrates with Docker and
Kubernetes, making it simple to run sandboxed containers.

Requirements
------------

* Docker
* containerd

Role Variables
--------------

Dependencies
------------

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: k8s-nodes
      roles:
         - { role: jonmosco.gvisor }

License
-------

BSD

Author Information
------------------

This role was created by Jon Mosco in 2022.
