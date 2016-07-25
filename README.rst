OpenStack-Ansible Galera Client
###############################
:tags: openstack, galera, client, cloud, ansible
:category: \*nix

This Ansible role installs the MariaDB operating system and Python packages
used to interact with and manage a Galera cluster.

Required Variables
------------------

To use this role, define the following variables:

.. code-block:: yaml

    galera_root_password: secrete

Dependencies
------------

This role depends on the ``config_template`` Ansible module provided
by `OpenStack-Ansible Plugins`_

.. _OpenStack-Ansible Plugins: https://github.com/openstack/openstack-ansible-plugins

Example Playbook
----------------

.. code-block:: yaml

    - name: Install Galera Client
      hosts: all
      user: root
      roles:
        - role: "openstack-ansible-galera_client"
          galera_address: "10.0.0.1"
          galera_root_password: secrete
          galera_root_user: root
          galera_client_drop_config_file: true

