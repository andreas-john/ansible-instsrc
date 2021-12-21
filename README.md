Role Name
=========

download, extract, configure, make and make install.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.
run as root for the finishing make install command -> -bK 

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

user 	.. mandatory, user which contains the target source dir
src_dir	.. mandatory, directory in which the package is downloaded and extracted
url 	.. mandatory, url to download the packaged source (tar.gz, tgz,...)
sha	.. optional, url to sha checksum file for downloaded source
cleanup	.. optional, remove all artefacts after make install

Dependencies
------------

none

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
Andreas JOHN, incinerator at gmx.at
