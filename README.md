troykinsella.docker-swarm
=========================

An ansible role to install a docker-swarm binary by docker image pull.

Role Variables
--------------

* docker_swarm_container_name: The name of the swarm docker container. Default: swarm.
* docker_swarm_image_name: The name of the swarm docker image: Default: swarm.
* docker_swarm_binary_path: The full path to the installed docker-swarm binary. Default: /usr/local/bin/docker-swarm.
* docker_swarm_binary_mode: The file mode of the docker-swarm binary. Default: 0755.
* docker_swarm_binary_user: The docker-swarm binary user. Default: root.
* docker_swarm_binary_group: The docker-swarm binary group. Default: root.
* docker_swarm_lazy_install: Yes to pull the swarm image upon the first execution of the binary. Default: yes.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: troykinsella.docker-swarm

License
-------

MIT




Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
