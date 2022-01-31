# Amtega git_commit role

This is an [Ansible](http://www.ansible.com) role to commit changes in a git repository.

## Role Variables

A list of all the default variables for this role is available in `defaults/main.yml`. The role setup the following facts:

- `git_commit_result`: result of the git commit

## Example Playbook

This is an example playbook:

``` yaml
---
- hosts: localhost
  roles:  
    - amtega.git_commit
  vars:    
  vars:
    git_commit_repo_dir: /tmp/git_commit
    git_commit_message: Ansible git_commit role test.
    git_commit_add_changes: yes
```

## Testing

Tests are based on [molecule with docker containers](https://molecule.readthedocs.io/en/latest/installation.html).

```shell
cd amtega.git_commit

molecule test --all
```

## License

Copyright (C) 2022 AMTEGA - Xunta de Galicia

This role is free software: you can redistribute it and/or modify it under the terms of:

GNU General Public License version 3, or (at your option) any later version; or the European Union Public License, either Version 1.2 or – as soon they will be approved by the European Commission ­subsequent versions of the EUPL.

This role is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details or European Union Public License for more details.

## Author Information

- Juan Antonio Valiño García.
