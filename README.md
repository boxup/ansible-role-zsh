zsh
===

An Ansible role to install and setup zsh

Requirements
------------

None.

Role Variables
--------------

- zsh_install_options: disable-etcdir
    - install options for homebrew zsh
- zsh_set_login_shell: yes
    - whether or not to set zsh as the login shell

- zsh_zprezto_setup: yes
    - whether or not to setup zprezto
- zsh_zprezto_git_url: https://github.com/sorin-ionescu/prezto.git
    - the url of zprezto git repository
- zsh_zprezto_work_dir: ~/.zprezto
    - the install target directory of zprezto

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
