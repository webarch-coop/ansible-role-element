# Webarchitects Element Ansible role

An Ansible role to install and configure the [Element](https://github.com/vector-im/element-web) Matrix web client.

## Defaults

The following [defaults/main.yml](defaults/main.yml) are defined:

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
