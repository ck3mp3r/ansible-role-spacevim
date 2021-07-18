Role Name
=========
SpaceVim

Requirements
------------
Package manager for relevant distro or if on Darwin homebrew needs to be available. Only required when using `with_neovim: true`.
Package manager for either/or python, nodejs and ruby need to be available when using `with_neovim_support_for`.

Role Variables
--------------
```
with_neovim: false
```
If set to true it will attempt to install neovim with whatever package manager is available.

```
with_neovim_support_for: []
```
Possible values for the list are ['nodejs', 'python', 'ruby']

Example Playbook
----------------

    - hosts: localhost
      connection: local
      roles:
         - { role: ck3mp3r.spacevim, with_neovim: true, with_neovim_support_for: ['nodejs'] }

License
-------

MIT

Author Information
------------------

Christian Kemper | kemper.buzz
