Ansible Role: kail
==================

Role to download and install [kail](https://github.com/boz/kail) Kubernetes CLI that
 lets you view logs in style

Requirements
------------

* Ansible >= 2.7

* Linux Distribution

    * Debian Family

        * Debian

            * Jessie (8)
            * Stretch (9)

        * Ubuntu

            * Xenial (16.04)
            * Bionic (18.04)

    * RedHat Family

        * CentOS

            * 7

    * Note: other versions are likely to work but have not been tested.

Role Variables
--------------

The following variables will change the behavior of this role (default values
are shown below):

```yaml
# kail version number
kail_version: '0.15.0'


Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: istvano.kail
```

Development & Testing
---------------------

This project uses [Molecule](http://molecule.readthedocs.io/).

You can test it by running with the provided

[Molecule Wrapper](https://github.com/gantsign/molecule-wrapper).

```bash
./moleculew test
```

If you want to lint the project use:
```bash
./moleculew lint
```

or you can test it locally by running

```bash
ansible-playbook ./tests/test.yml
```

License
-------

MIT
