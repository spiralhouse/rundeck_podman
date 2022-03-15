rundeck-podman
=========

Ansible role to install and manage [Rundeck](https://www.rundeck.com/) containers with [Podman](https://podman.io/) and [systemd](https://freedesktop.org/wiki/Software/systemd/). 

### Important limitations: 
* In proof of concept phase. It works, but is poorly documented and needs much to be ironed out before publishing.
* Only tested with Debian and Ubuntu. Pull requests with contributions for other distros welcome!
* Only supports Rundeck Community Edition. No Enterprise (yet).
* Only supports built-in H2 database, not suited for production.

Requirements
------------

* A Linux system capable of running podman and systemd. In theory:
  * Debian / Ubuntu (tested)
  * RHEL / CentOS
  * Fedora
  * openSUSE
  * Gentoo
  * Arch Linux
* Rundeck itself requires the following minimum system resources:
  * 2 CPUs
  * 4 GB RAM
  * 20 GB hard disk

Role Variables
--------------

TBD

Dependencies
------------

### Roles:
  * [ikke_t.podman_container_systemd]()

### Collections:
  * [containers.podman]()
  * [ansible.posix]()

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

GPLv3

Author Information
------------------

John Burbridge - [john@spiralhouse.io](mailto:john@spiralhouse.io)
