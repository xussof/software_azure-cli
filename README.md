software_azure-cli
=========

This role will install azure-cli software

Requirements
------------

All dependencies will appear on requirements.yml file
Role Variables
--------------

Not defined yet. But in the future we could stage software version in here

Dependencies
------------

All dependencies will appear on requirements.yml file

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    #ansible-playbook test-software.yml --extra-vars "ansible_become_pass={{ sudo_pass }}"
    - hosts: localhost
      pre_tasks:
        - raw: ansible-galaxy install -f -r requirements-software.yml
        - raw: ansible-galaxy install -f -r software_azure-cli/requirements.yml
      vars_files:
        - "encrypted.yml"

      tasks:
        - name: Including role to test
          include_role:
            name: software_azure-cli


License
-------

BSD

Author Information
------------------
Made by @xussof
