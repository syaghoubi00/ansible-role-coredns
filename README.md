# CoreDNS

Installs [CoreDNS](https://coredns.io/)
([GitHub](https://github.com/coredns/coredns))

## Requirements

None.

## Role Variables

`coredns_auto_update: false` - don't automatically update to latest by default

`coredns_group: "coredns"` - name of coreDNS group

`coredns_port: 53` - port CoreDNS will listen on

`coredns_user: "coredns"` - name of CoreDNS user

`coredns_version: null` - undefined will use `latest`

### TODO

Add variable to install in a container

## Dependencies

None.

## Example Playbook

```yaml
- hosts: dns_servers
  vars:
  roles:
    - syaghoubi00.coredns
```

## License

GPL-3.0-or-later

## Author Information

Created by Sebastian Yaghoubi
