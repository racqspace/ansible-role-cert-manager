# Ansible Role: cert_manager

![MIT](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/racqspace/ansible-role-cert-manager/Main?style=flat-square)
![GitHub last commit](https://img.shields.io/github/last-commit/racqspace/ansible-role-cert-manager?style=flat-square)
![GitHub Release Date](https://img.shields.io/github/release-date/racqspace/ansible-role-cert-manager?style=flat-square)
![Maintenance](https://img.shields.io/maintenance/yes/2022?style=flat-square)

Installing cert_manager in Kubernetes.

## Role Variables

Variable Name | Default Value | Description
------------ | ------------- | -------------
cert_manager_cache_valid_time | 3600 | Cache update time for apt module.
cert_manager_namespace | default | Specify the kubernetes namespace to install resources to.

## Role Usage Examples

Example for installing cert_manager in a dedicated namespace `cert_manager`.

```yaml
- hosts: all
  roles:
  - role: racqspace.cert_manager
    vars:
      cert_manager_namespace: cert_manager
```

## License

MIT

## Author Information

This role was created in 2021 by [Clemens Kaserer](https://www.ckaserer.dev/).

Contributions by:

- [@ckaserer](https://github.com/ckaserer)
