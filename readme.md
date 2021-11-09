Profile Role
=========

A brief description of the role goes here.

[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-neoloc.profile-blue.svg)](https://galaxy.ansible.com/neoloc/ansible-role-profile/)


Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

An example list of all variables for this role should go here, including any variables that are in defaults/main.yml and vars/main.yml. Any variables that are read from other roles and/or the global scope (e.g. hostvars, groupvars, etc) should be shown here also.


```yaml
profile_profile_d_files:
  00_path:
    content: content |
      PATH="$PATH:/usr/local/sbin:/usr/sbin:/sbin"
      export PATH
```

This will create the `/etc/profile.d/00_path.sh` file with the following contents:

```bash
PATH="$PATH:/usr/local/sbin:/usr/sbin:/sbin"
export PATH
```

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - neoloc.profile

License
-------

See license.md

Author Information
------------------

[![Github](https://img.shields.io/badge/Github-neoloc-blue.svg)](https://github.com/neoloc)
