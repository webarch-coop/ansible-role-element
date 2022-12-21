# Webarchitects Element Ansible role

An Ansible role to install and configure the [Element](https://github.com/vector-im/element-web) Matrix web client, see also the [synapse-server](https://git.coop/webarch/synapse-server) repo for an example of how to use this role.

## Role variables

See the [defaults/main.yml](defaults/main.yml) file for the default variables and [meta/argument_spacs.yml](meta/argument_specs.yml) for the variable specification.

### element

`element` a boolean, when `true` tasks in this role are run, it defaults to `false`.

### element_ca_path

`element_ca_path` is the path to the TLS certificate authority (CA) certificate for the `element_domain`.

### element_cert_path

`element_cert_path` is the path to the TLS certificate for the `element_domain`.

### element_config

`element_config` is a YAML dictionary that is written as JSON for the Element configuration.

### element_domain

`element_domain` is the domain name that the Element website wil be hosted on.

### element_domain_redirects

`element_domain_redirects` is list of domain names to redirect to the `element_domain`.

### element_matrix_domain

`element_matrix_domain` is the domain name of the Matrix Synapse server.

### element_key_path

`element_key_path` is the path to the TLS key for the `element_domain`.

### element_version

`element_version` is the version of Element to install, this can either be set to `latest`, the default or [a version number](https://github.com/vector-im/element-web/releases).

## Dependencies

This role requires Ansible `2.13` or newer plus [JC](https://pypi.org/project/jc/) and [JMESPath](https://pypi.org/project/jmespath/) to be installed using `pip3` on the Ansible controller.

## Repository

The primary URL of this repo is [`https://git.coop/webarch/element`](https://git.coop/webarch/element) however it is also [mirrored to GitHub](https://github.com/webarch-coop/ansible-role-element) and [available via Ansible Galaxy](https://galaxy.ansible.com/chriscroome/element).

If you use this role please use a tagged release, see [the release notes](https://git.coop/webarch/element/-/releases).

## License

This role is released under [the same terms as Ansible itself](https://github.com/ansible/ansible/blob/devel/COPYING), the [GNU GPLv3](LICENSE).
