galera_client Docs
==================

Installation of the mariadb client used for galera clusters.

Basic Role Example
^^^^^^^^^^^^^^^^^^

.. code-block:: yaml

    - name: Install galera server
      hosts: galera_all
      user: root
      roles:
        - role: "galera_server"
          galera_address: "10.0.0.1"
          galera_root_password: secrete
          galera_root_user: root
