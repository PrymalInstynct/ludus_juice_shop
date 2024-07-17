# Ansible Role: Juice Shop ([Ludus](https://ludus.cloud))

An Ansible Role that will deploy the OWASP Juice Shop Vulnerable Web Application using NPM

## Requirements

- community.general

## Role Variables

None.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: hosts
  roles:
    - PrymalInstynct.ludus_juice_shop
```

## Example Ludus Range Config

```yaml
ludus:
  - vm_name: "{{ range_id }}-juice"
    hostname: "{{ range_id }}-juicer"
    template: debian-12-x64-server-template
    vlan: 10
    ip_last_octet: 1
    ram_gb: 4
    cpus: 2
    linux: true
    roles:
      - PrymalInstynct.ludus_juice_shop
```

## License

GPLv3

## Author Information

This role was created by [PrymalInstynct](https://github.com/PrymalInstynct), for [Ludus](https://ludus.cloud/).
