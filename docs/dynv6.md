# DynV6

## Configuration

### Example

```json
{
  "settings": [
    {
      "provider":"dynv6",
      "domain":"dns.navy",
      "host":"yourhosthere",
      "token":"tokenxxxxxxxxx",
      "ip_version":"ipv4",
      "ipv6_suffix":""
    }
  ]
}


```
this is fix 9.11.2024 - working for dynv6
### Compulsory parameters

- `"domain"` is the domain to update. It can be `example.com` (root domain) or `sub.example.com` (subdomain of `example.com`).
- `"token"` that you can obtain [here](https://dynv6.com/keys#token)

### Optional parameters

- `"ip_version"` can be `ipv4` (A records), or `ipv6` (AAAA records) or `ipv4 or ipv6` (update one of the two, depending on the public ip found). It defaults to `ipv4 or ipv6`.
- `"ipv6_suffix"` is the IPv6 interface identifier suffix to use. It can be for example `0:0:0:0:72ad:8fbb:a54e:bedd/64`. If left empty, it defaults to no suffix and the raw public IPv6 address obtained is used in the record updating.

## Domain setup
