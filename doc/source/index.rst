===============================
OpenStack-Ansible Galera client
===============================

This Ansible role installs packages used to interact with and manage a Galera
cluster.

To clone or view the source code for this repository, visit the role repository
for `galera_client <https://opendev.org/openstack/openstack-ansible-galera_client>`_.

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

This role needs pip >= 7.1 installed on the target host.

This role depends on the ``config_template`` Ansible module provided
by `OpenStack-Ansible Plugins`_.

.. _OpenStack-Ansible Plugins:
   https://opendev.org/openstack/openstack-ansible-plugins

Example playbook
~~~~~~~~~~~~~~~~

.. literalinclude:: ../../examples/playbook.yml
   :language: yaml
