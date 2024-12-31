# CoreDNS

Installs [CoreDNS](https://coredns.io/)
([GitHub](https://github.com/coredns/coredns))

## Requirements

None.

## Role Variables

`coredns_auto_update: false` - Don't automatically update to `latest` by default

`coredns_config:` - Use an inline configuration

`coredns_corefile:` - Use a config from file

`coredns_group: "coredns"` - The name of the CoreDNS group

`coredns_health_check_enabled: true` - CoreDNS health check endpoint enabled

`coredns_health_check_port: 8091` - Port that the CoreDNS health check endpoint
will listen on

`coredns_install_method: binary` - How CoreDNS will be installed, `binary` or
`container` (_container install not implemented yet_)

`coredns_port: 53` - What port CoreDNS will listen on

`coredns_user: "coredns"` - The name of the CoreDNS user

`coredns_version: null` - `undefined` will use `latest`

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
