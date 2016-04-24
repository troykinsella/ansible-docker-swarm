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
