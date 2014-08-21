zsh
===

An Ansible role to install and setup zsh

Requirements
------------

None.

Role Variables
--------------

- epel_base_url: The base url of the EPEL repository. The default value is http://ftp.iij.ad.jp/pub/linux/fedora/epel

- zsh_install_options: disable-etcdir
    - install options for homebrew zsh
- zsh_set_login_shell: yes
    - whether or not to set zsh as the login shell

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: hnakamur.zsh, zsh_install_options: "" }

License
-------

MIT

Author Information
------------------

[Hiroaki Nakamura]( http://hnakamur.github.io/ )
