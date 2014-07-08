# ngircd

Install ngircd and generate self-signed certificate.

## Requirements

- Ubuntu
- Debian

## Role Variables

- `ngircd_hostname`
- `[Global]`
  - `ngircd_network_name`
  - `ngircd_admin_info1`
  - `ngircd_admin_info2`
  - `ngircd_admin_email`
  - `ngircd_info`
  - `ngircd_listen`
  - `ngircd_password`
  - `ngircd_ports`
- `[Limits]`
  - `ngircd_max_nick_length`
- `[SSL]`
  - `ngircd_ssl_cert_file`
  - `ngircd_ssl_dh_file`
  - `ngircd_ssl_key_file`
  - `ngircd_ssl_ports`
- role only
  - `ngircd_ssl_csr_file`
  - `ngircd_ssl_csr_subj`

## Dependencies

None.

## Example Playbook

    ---
    - hosts: servers
      roles:
         - { role: znzj.ngircd }

## License

MIT License
