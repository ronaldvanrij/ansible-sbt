# Ansible Role: jeffhung.sbt

Ansible playbook for installing SBT on CentOS/Debian Linux

Install this playbook:

	ansible-galaxy install jeffhung.sbt


## Role Variables

### `sbt_version`

Default: `0.13.12`

Set which version to use.

### `sbt_environment`

Default: `devel`

Which environment to deploy.

Could be:

* `devel`: provision devel-time environment for developing
* `build`: provision build-time environment for packaging

### `sbt_install_from`

Choose the source where maven is installed from.

Could be:

* `binaries`: install from released binary tarball
* `packages`: install from automatically downloaded RPM/DEB packages (n/a)
* `repositories`: install from YUM/APT repositories

Default: `repositories`

### `sbt_cache_dir`

Cache directory for holding downloaded/generated files.

The default is `/vagrant/files` so cache persist between boxes.


## License

BSD

