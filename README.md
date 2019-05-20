# Ansible Role: BBR

An Ansible Role that enable BBR on Linux with kernel 4.9+.

## Requirements

Kernel 4.9+

## Role Variables

None

## Dependencies

None.

## Example Playbook

```yaml
---
- hosts: all
  remote_user: sysops
  become: yes
  # remote_user: user
  # become: yes
  # become_method: sudo
  roles:
    - role: 'bbr'
```

Then run the playbook, like this:

```shell
ansible-playbook -i hosts bbr.yml
```

If use a SSH Key with custom name, run the playbook like this:

```shell
ansible-playbook -i hosts bbr.yml  --become --key-file ~/.ssh/vps-ssh-key
```

## License

MIT / BSD

## Author Information

This role was created by [小碼哥](https://thisiswangle.com/)
