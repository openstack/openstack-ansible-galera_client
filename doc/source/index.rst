===============================
OpenStack-Ansible Galera client
===============================

This Ansible role installs the MariaDB operating system and Python
packages used to interact with and manage a Galera cluster.

Default variables
~~~~~~~~~~~~~~~~~

.. literalinclude:: ../../defaults/main.yml
   :language: yaml
   :start-after: under the License.

Required variables
~~~~~~~~~~~~~~~~~~

To use this role, define the following variables:

.. code-block:: yaml

    galera_root_password: secrete

Dependencies
~~~~~~~~~~~~

This role depends on the ``config_template`` Ansible module provided
by `OpenStack-Ansible Plugins`_.

.. _OpenStack-Ansible Plugins:
   https://git.openstack.org/cgit/openstack/openstack-ansible-plugins

Example playbook
~~~~~~~~~~~~~~~~

.. literalinclude:: ../../examples/playbook.yml
   :language: yaml
